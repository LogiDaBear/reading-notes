# In memory Storage

1. What is a ‘call’?
- At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).
2. How many ‘calls’ can happen at once?
- One at a time
3. What does LIFO mean?
- Last In First Out

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
    [call stack](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)
5. What causes a Stack Overflow?
- A stack overflow occurs when there is a recursive function(a function calls itself) without an exit point.
ex:
          function callMyself(){
            callMyself();
          }

          callMyself();

## Things I want to learn more about 
- CSS always :D