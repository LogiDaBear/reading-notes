# Pythonisms

## What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.

Dunder methods, short for "double underscore" methods, are special methods in Python that enable customization of built-in behaviors within classes. These methods are also known as magic methods or special methods. They are enclosed by double underscores at the beginning and end of their names, such as `__init__` for initialization. Dunder methods allow developers to define how objects of a class should behave in response to various operations, such as addition, subtraction, string representation, and more. For instance, the `__str__` dunder method is used to customize the string representation of an object when it's converted to a string using the `str()` function or through string interpolation. By implementing dunder methods, programmers can tailor the behavior of their custom classes to fit specific requirements.

## Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

An iterator in Python is a way to access elements in a sequence one by one. It's like a cursor that moves through a collection of items. To create a custom iterator, you use the `iter()` and `next()` methods. The `iter()` method is used to make an object iterable, and the `next()` method is used to fetch the next item in the sequence. These methods are crucial for enabling iteration in a class because they allow you to control how your objects are iterated over. By defining these methods, you can specify what happens when you loop through instances of your class, making your class more versatile and usable in different scenarios.

## What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.

A generator in Python is a special type of function that generates values on-the-fly and allows for memory-efficient iteration over large datasets or infinite sequences. It differs from a regular function in that it doesn't necessarily compute and return all values at once. Instead, it yields one value at a time using the `yield` keyword, maintaining its internal state between calls. This makes generators more memory-efficient since they don't store the entire sequence in memory.

Here's an example of a generator function that generates a sequence of Fibonacci numbers:

```python
def fibonacci_generator():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

# Using the generator to generate Fibonacci numbers
fib_gen = fibonacci_generator()
for _ in range(10):
    print(next(fib_gen))
```

- When you call `next(fib_gen)`, it computes and yields the next Fibonacci number in the sequence, maintaining its internal state between calls. This allows you to generate an indefinite number of Fibonacci numbers without needing to store them all in memory at once.

## Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.


Decorators in Python are a powerful way to modify or enhance the behavior of functions or methods without changing their code. They allow you to wrap a function with additional functionality. The primary use case for decorators is to add features like logging, access control, or caching to functions in a clean and reusable manner. To create a custom decorator, you define a function that takes another function as its argument. Inside the decorator function, you typically perform some actions before and/or after calling the original function, and you return the result. You then apply the decorator using the `@decorator_name` syntax above the function you want to enhance. For example, to create a simple timing decorator:

```python
import time

def timing_decorator(func):
    def wrapper(*args, **kwargs):
        start_time = time.time()
        result = func(*args, **kwargs)
        end_time = time.time()
        print(f"Time taken: {end_time - start_time} seconds")
        return result
    return wrapper

@timing_decorator
def slow_function():
    time.sleep(2)

slow_function()
```

## things I want to know more about
[Decorators](https://realpython.com/primer-on-python-decorators/)