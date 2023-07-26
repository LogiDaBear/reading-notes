# Authentication and Production Server

## What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

JWTs are used for secure data transmission between parties. They act as digitally signed tokens to validate the authenticity of information. They work by encoding data into a JSON format, signing it with a secret key, and then sending it. The recipient can decode and verify the signature to trust the data.

## How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT Authentication in Django REST Framework is used to secure API endpoints. Key components involved are: `djangorestframework-simplejwt ` library for JWT support, `TokenObtainPairView `to get tokens, and `TokenVerifyView` to validate tokens in requests.

## Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django's built-in runserver is not suitable for production due to limited features, poor performance, and security risks. Alternative server options include Gunicorn, uWSGI, and ASGI servers like Daphne, suitable for deploying Django apps.