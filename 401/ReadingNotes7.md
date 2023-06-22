# List Comprehension
## What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.
  - `my_new_list = [ expression for item in list ]`

  - Using a for loop would require more code and is generally less concise than using a list comprehension.

 - ```create a list using list comprehension
squares = [x**2 for x in range(10)]

print(squares)```

## What is a decorator in Python?

  - Decorators are commonly used for adding logging, timing, authentication, or other cross-cutting concerns to functions or classes without modifying their original code. They provide a flexible way to extend and modify the behavior of Python functions and classes. Decorators are implemented using the @ symbol followed by the decorator function or class name placed above the function or class definition.

  ```from decorators import do_twice

@do_twice
def say_whee():
    print("Whee!")
When you run this example, you should see that the original say_whee() is executed twice:

>>> say_whee()
Whee!
Whee!```

## Things I want to know more about

[Parsing a file using list comprehension](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python#htoc-parsing-a-file-using-list-comprehension)