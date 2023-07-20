# Django Custom User

## What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?

Using a Django Custom User Model provides several benefits, including enhanced flexibility, scalability, and integration with existing systems. It allows you to tailor the user model to match the project's specific needs, optimize database performance, and implement custom authentication methods for improved security. Moreover, Custom User Models enable the creation of multiple user types with distinct fields and functionalities. In contrast, the default Django User Model is more limited, requiring extensions through a separate profile model and posing challenges for field modifications. Ultimately, a Custom User Model offers a more robust and customizable solution for handling user-related aspects in Django applications.

## Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.

create a new django app: pmp startapp blah, define the custom user model in models.py:
```
    from django.contrib.auth.models import AbstractBaseUser, BaseUserManager, PermissionsMixin
from django.db import models
from django.utils import timezone

class CustomUserManager(BaseUserManager):
    def create_user(self, email, password=None, **extra_fields):
        if not email:
            raise ValueError("The Email field must be set")
        email = self.normalize_email(email)
        user = self.model(email=email, **extra_fields)
        user.set_password(password)
        user.save(using=self._db)
        return user

    def create_superuser(self, email, password=None, **extra_fields):
        extra_fields.setdefault('is_staff', True)
        extra_fields.setdefault('is_superuser', True)

        if extra_fields.get('is_staff') is not True:
            raise ValueError('Superuser must have is_staff=True.')
        if extra_fields.get('is_superuser') is not True:
            raise ValueError('Superuser must have is_superuser=True.')

        return self.create_user(email, password, **extra_fields)

class CustomUser(AbstractBaseUser, PermissionsMixin):
    email = models.EmailField(unique=True)
    first_name = models.CharField(max_length=30, blank=True)
    last_name = models.CharField(max_length=30, blank=True)
    date_joined = models.DateTimeField(default=timezone.now)
    is_active = models.BooleanField(default=True)
    is_staff = models.BooleanField(default=False)

    USERNAME_FIELD = 'email'
    REQUIRED_FIELDS = []

    objects = CustomUserManager()

    def __str__(self):
        return self.email
```
update settings.py to use the custom user model: AUTH_USER_MODEL = 'blah_user.CustomUser',
pmp makemigrations
pmp migrate

finally we update admin.py
```
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin
from .models import CustomUser

admin.site.register(CustomUser, UserAdmin)

```
## What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.


DjangoX is a Django starter project that includes a number of features that can help you get started with your project more quickly. These features include user authentication, static files configuration, styling with Bootstrap, debugging with django-debug-toolbar, DRY forms with django-crispy-forms, and custom 404, 500, and 403 error pages. DjangoX can complement or extend the functionality of Django by providing these features out of the box, which can save you time and effort when you are getting started with your project. For example, if you are creating a new website that requires user authentication, you can use DjangoX to get started with user login, registration, and password reset functionality. Another example is if you are creating a new website that uses Bootstrap for styling. DjangoX includes Bootstrap v5 out of the box, so you can start using it right away. Overall, DjangoX is a great way to get started with a new Django project.

## Things I want to know more about
What was life like without Django