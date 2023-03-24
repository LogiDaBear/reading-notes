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

# JS error messages

1. What is a ‘reference error’?
- When you try and use a variable that is not yet declared you get this error
2. What is a ‘syntax error’?
- this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
3. What is a ‘range error’?
- Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
4. What is a ‘type error’?
- this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
5. What is a breakpoint?
- If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.
6. What does the word ‘debugger’ do in your code?
- A breakpoint can be achieved by putting a debugger statement in your code in the line you want to break.

## Things I want to learn more about 
- CSS always :D