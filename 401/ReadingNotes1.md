# Reading Notes for Class 1
Pain v Suffering is hardcore and so am I. Lets do Python 401 BAYBEEEEE!

### random notes from [source](https://www.youtube.com/watch?v=_AEJHKGk9ns) material
Assignments never copy data. 
Immutable values cant alias and cannot mutate an int because they are immutable. 
Function arguements are assignments.

### bigO notes
- O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

  ```bool IsFirstElementNull(IList<String> elements)
    {
        return elements[0] == null;
    }

- O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set. The example below also demonstrates how Big O favours the worst-case performance scenario; a matching string could be found during any iteration of the for loop and the function would return early, but Big O notation will always assume the upper limit where the algorithm will perform the maximum number of iterations.

  ```bool ContainsValue(IEnumerable<string> elements, string value)
    {
        foreach (var element in elements)
        {
            if (element == value) return true; 
        }     
        return false; 
    }

- O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N³), O(N⁴) etc.

  ```bool ContainsDuplicates(IList<string> elements)
    {
        for (var outer = 0; outer < elements.Count; outer++) 
        {
            for (var inner = 0; inner < elements.Count; inner++) 
            { 
                // Don't compare with self 
                if (outer == inner) continue;             
                
                if (elements[outer] == elements[inner]) return true; 
            }
        }    
        return false;
    }

- O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow, then rising meteorically. An example of an O(2^N) function is the recursive calculation of Fibonacci numbers:

   ``` int Fibonacci(int number)
    {
        if (number <= 1) return number;
          
        return Fibonacci(number - 2) + Fibonacci(number - 1); 
    }
## Reading
- [Pain vs Suffering](https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering)

- [BigO](https://robbell.io/2009/06/a-beginners-guide-to-big-o-notation)

## Things I want to know more about
Values live until reference is gone means... what?