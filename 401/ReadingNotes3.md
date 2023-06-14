# FileIO & Exceptions
## Reading/Videos
- [Read and Write files in Python](https://realpython.com/read-write-files-python/)
- [Exceptions in Python](https://realpython.com/python-exceptions/)
- [Reading and Writing to files video](https://www.youtube.com/watch?v=Uh2ebFW8OYM)

1. What is the purpose of the `with` statement when opening a file in Python, and how does it help manage resources while reading and writing files?

- 
The purpose of the `with` statement when opening a file in Python is to ensure that the file is properly closed after its use. It helps manage resources by automatically handling the process of opening and closing the file, even if an exception occurs.

2. Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

- the `read()` method is used to read the entire content of a file, while the `readline()` method is used to read individual lines.

3. Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

- try block:
The 'try' block is where you place the code that might raise an exception. It is followed by one or more 'except' blocks that define how to handle specific exceptions.

- except block:
An 'except' block is used to catch and handle specific exceptions that occur within the preceding 'try' block. You can have multiple 'except' blocks to handle different types of exceptions or to provide different handling logic based on the type of exception encountered.

- finally block:
The 'finally' block is optional and is used to define code that should be executed regardless of whether an exception occurred or not. It is typically used to perform cleanup operations like closing files or releasing resources.


```try:
    x = int(input("Enter a number: "))
    result = 10 / x
    print("Result:", result)
except ValueError:
    print("Invalid input. Please enter a valid number.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
finally:
    print("End of program.")
```

## Things I want to know more about
