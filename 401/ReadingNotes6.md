## Variable Scope in Python

In Python, **variable scope** refers to the region or part of the program where a variable is accessible or visible. The scope determines the lifespan and accessibility of a variable within a program.

Python has two main types of variable scope:

1. **Local Scope:** Variables defined within a function or block have local scope. They are accessible only within that specific function or block and are destroyed when the function or block execution ends. Local variables cannot be accessed from outside the function or block.

2. **Global Scope:** Variables defined outside of any function or block have global scope. They are accessible throughout the entire program, including all functions and blocks. Global variables retain their value as long as the program is running.


## Global and Nonlocal Keywords in Python

1. **Global Keyword:**
   - The **global** keyword is used to declare that a variable inside a function is a global variable, allowing it to be accessed and modified within that function and outside of it.
   - When you assign a value to a variable inside a function without using the **global** keyword, Python creates a new local variable with the same name instead of modifying the global variable.
   - The **global** keyword allows you to explicitly specify that a variable refers to the global scope, ensuring that the global variable is accessed and modified.
   - The **global** keyword is typically used when you want to modify a global variable inside a function.

2. **Nonlocal Keyword:**
   - The **nonlocal** keyword is used to access variables from the outer (enclosing) local scope in nested functions.
   - When a variable is defined in the inner function and shares the same name as a variable in the outer function, the inner function's variable usually shadows the outer function's variable.
   - By using the **nonlocal** keyword, you can explicitly state that a variable is not local to the inner function and should refer to the variable in the outer function.
   - The **nonlocal** keyword is typically used in nested functions when you want to modify a variable from an outer scope.

You might use the **global** keyword when you want to modify a global variable from within a function. This can be useful when you need to update global state or configuration settings.

You might use the **nonlocal** keyword when you have nested functions, and you want to modify a variable from an outer scope inside the inner function. This is useful when you need to maintain state or access variables from the enclosing scope.

## Purpose and Importance of Big O Notation in Algorithm Analysis

1. **Efficiency Comparison:** Big O notation allows us to compare different algorithms and understand which algorithm is more efficient in terms of time complexity or space complexity. It provides a common language to discuss and reason about algorithmic efficiency.

2. **Scalability Understanding:** Big O notation can predict how an algorithm will perform as the input size increases. It helps in understanding how algorithms scale and how they will handle larger datasets or more complex scenarios.

3. **Algorithm Selection:** Big O notation assists in choosing the most appropriate algorithm for a specific task or problem. By considering the Big O complexity, select an algorithm that meets the performance requirements and constraints of the problem.

4. **Optimization Guidance:** Big O notation helps identify areas in their algorithms that may be inefficient or have room for improvement. It provides insights into which parts of the algorithm may have a higher impact on performance and where optimization efforts should be focused.

5. **Algorithm Design:** Big O notation encourages you to think about and analyze the efficiency of the algorithm designs. It promotes the development of algorithms that are efficient and scalable, leading to better software solutions.


## Based on the Rolling Dice Example
- import random and print random.randint`(1,6))`
`import random
count = 0

def roll():
    return random.randint(1,6)

for i in range(1, 1001):
    if roll() == 6:
        count += 1`

- using code to calculate the probability of rolling a specified number over a large number of trails you can create variables that `target_a_number` and do a `number_of_trials` and then calculate something like this 
`   for _ in range(num_trials):
        result = roll_dice()
        if result == target:
            count += 1
    probability = count / num_trials
    return probability`
## Things I want to know more about
linked lists