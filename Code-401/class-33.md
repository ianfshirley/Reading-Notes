## DRF Authentication & Production Server

### Introduction to JSON Web Tokens

- compact and self-contained way for securely transmitting information between parties as a JSON object. 
- useful for authorization & information exchange
- structure:
  - header
  - payload
  - signature

### How to Use JWT Authentication with Django REST Framework

- authorization token that should be included in every request
- acquired by exhanging username & password for access token and refresh token


### Django Runserver Is Not Your Production Server

- the built-in python server is not meant to be used in a production setting, it has not gone through security audits or performance tests
- use a server that's reliable, well-tested and has been around for a while
- be sure to use a production-ready web server like Nginx, and and application server like Gunicorn



### Sources

[Introduction to JSON Web Tokens](https://jwt.io/introduction/)<br>
[How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)<br>
[Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)<br>
[Gunicorn](https://gunicorn.org/)<br>
[Django Migrations: A Primer](https://realpython.com/django-migrations-a-primer/)<br>