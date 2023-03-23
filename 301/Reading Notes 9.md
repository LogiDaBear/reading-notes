# Functional Programming

1. What is functional programming?
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

2. What is a pure function and how do we know if something is a pure function?
- It returns the same result if given the same arguments (it is also referred as deterministic)

- It does not cause any observable side effects

3. What are the benefits of a pure function?
 Easier code to test

4. What is immutability?
 Unchanged behavior or unable to be changed
 - When data is immutable, its state cannot change after it’s created.

5. What is Referential transparency?
- pure functions + immutable data = referential transparency
# Node JS

1. What is a module?
- Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application

2. What does the word ‘require’ do?

    The main object exported by the require module is a function (as used in the above example). When Node invokes that require() function with a local file path as the function’s only argument, Node goes through the following sequence of steps:

- Resolving: To find the absolute path of the file.
- Loading: To determine the type of the file content.
- Wrapping: To give the file its private scope. This is what makes both the require and module objects local to every file we require.
- Evaluating: This is what the VM eventually does with the loaded code.
- Caching: So that when we require this file again, we don’t go over all the steps another time.


3. How do we bring another module into the file the we are working in?
- use the require keyword at the top of the file

4. What do we have to do to make a module available?
    Creating Node. js modules
    Overview.
    Create a package.json file.
    Create the file that will be loaded when your module is required by another application.
    Test your module.
    Resources.
