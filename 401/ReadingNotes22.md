# Permissions & Postgresql

## What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

DRF Permissions are a set of rules that control access to resources in a Django REST API. They ensure that only authorized users can perform certain actions, like viewing, editing, or deleting data. These permissions help secure the API by restricting access based on user roles, authentication status, or custom conditions.

## In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

The SELECT statement is used in SQL to retrieve data from a database. It allows you to fetch specific information from one or more tables. The primary purpose of the SELECT statement is to query and retrieve data, which can be used for analysis, display, or further processing.

Using SELECT to retrieve all columns from the 'employees' table:
To retrieve all columns from the 'employees' table, you would use the following SQL query:

```
SELECT * FROM employees;
```
This query will return all rows and columns from the 'employees' table, giving you complete information about each employee stored in that table.

## Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

DRF Generic Views are pre-built views provided by Django Rest Framework to simplify the process of building RESTful APIs. They offer commonly used functionalities like retrieving a list of objects, retrieving a single object, creating a new object, updating an existing object, and deleting an object. These views abstract away common patterns and provide a streamlined way to handle typical API operations.

```
ChatGPT rendered example:
# views.py
from rest_framework.generics import ListCreateAPIView, RetrieveUpdateDestroyAPIView
from .models import Book
from .serializers import BookSerializer

# ListCreateAPIView for getting a list of books and creating a new book
class BookListCreateView(ListCreateAPIView):
    queryset = Book.objects.all()
    serializer_class = BookSerializer

# RetrieveUpdateDestroyAPIView for getting, updating, and deleting a single book
class BookDetailAPIView(RetrieveUpdateDestroyAPIView):
    queryset = Book.objects.all()
    serializer_class = BookSerializer

#In this example, we use DRF Generic Views to create views for handling a list of books and individual book details. These views automatically handle common HTTP methods like GET, POST, PUT, and DELETE, making it easier to build a RESTful API for the 'Book' model.
```

## Things I want to know more about
serializers