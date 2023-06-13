# Reading Notes for class 2

1. What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?
    - Test-Driven Development in Python follows key principles of writing tests first, testing for one behavior at a time, failing initially, writing minimal code, and refactoring. These principles contribute to the overall quality of code by improving code design, increasing test coverage, detecting bugs early, providing a faster feedback loop, and maintaining a clean and refactorable codebase.

2. Explain the purpose of the ```if __name__ == '__main__':``` statement in Python scripts. What are some use cases for including this conditional in your code?
    - 
The ```if __name__ == '__main__':``` statement in Python scripts is used to check if the current module is being run as the main program or if it is being imported as a module by another script. This conditional statement allows you to differentiate between the execution of a script as the main program and its use as a module.

The purpose of using ```if __name__ == '__main__': ``` is to provide a block of code that will only execute when the script is run directly as the main program. It allows you to define a set of instructions that should only be executed when the script is invoked directly from the command line or by clicking on it, rather than when it is imported by another script.

Use cases ```(from chatGPT as I felt it was explained better than the reading)``` are as follows:
  - Executing a script as a standalone program: When you want a particular piece of code to run only when the script is executed directly, you can place it within the if __name__ == '__main__': block. This ensures that the code within this block will not execute if the script is imported as a module.

  - Testing and debugging: You can include test code or debugging statements within the if __name__ == '__main__': block. This allows you to run   specific tests or debug statements when running the script directly, without affecting the behavior of the script when it is imported as a module.

  - Module initialization: You can use the if __name__ == '__main__': block to initialize the module and perform any necessary setup tasks when the script is executed directly. This can include setting up configurations, initializing variables, or loading required resources.

  - Code organization: Placing the main execution logic within the if __name__ == '__main__': block helps to separate it from the code that is intended to be used as a module. It improves code readability and makes it easier for other developers to understand how the script can be used as a standalone program.

3. Describe the concept of recursion in Python.
  - Recursion in Python is cleaner and easier to understand than while loops.They use LIFO (Last in first out) structure. It uses either recursive base or a base case.
  - Base case is used to terminate the recursive function so you are not stuck in loop hell
  - Each recursive call makes a new copy of that method in the stack memory, infinite recursion may lead to running out of stack memory
  - Examples of Recursive algorithms: Merge Sort, Quick Sort, Tower of Hanoi, Fibonacci Series, Factorial Problem, etc.

4. What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs.
- Modules:
    A module can be written in Python itself.
    A module can be written in C and loaded dynamically at run-time, like the re (regular expression) module.
    A built-in module is intrinsically contained in the interpreter, like the itertools module.
- Packages:
    Packages allow for a hierarchical structuring of the module namespace using dot notation. In the same way that modules help avoid collisions between global variable names, packages help avoid collisions between module names.
- Importing: To import a package or module, use the import statement followed by the package or module name.
If the package or module is located in the same directory as your script, you can simply import it by its name. For example, if you have a package named "my_package" with a module named "my_module.py", you can import it as follows:```import my_package.my_module```
[Read this](https://realpython.com/python-modules-packages/) and that will guide you. Or google it. Or chatgpt. Or stackoverflow. Or....

## Things I want to know more about
When to determine to create a package rather than individual modules. Also a more condensed and concise description of such because these reads were huge.

