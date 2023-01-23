## Intro to Django

### Getting Started with Django

- Models:
  - a model is the single, definitive source of information about your data. Generally, each model maps to a single database table.
  - each model is a Python class that is a subclass of django.db.models.Model
  - each attribute of the model represents a database field
  - with all of this django gives you an auto-generated database-access API
- URL Dispatcher:
  - Django allows you to design URLs however you want, with no framework limitations
  - to design URLs for an app, create a Python module called a URL configuration (URLconf). It maps between URL path expressions to Python functions
- Templates:
  - Django uses templates to generate HTMl dynamically
- Forms:
  - Django provides a powerful form library that handles rendering forms as HTML, validating user-submitted data, and converting that data to native Python types. It also provides a way to generate forms from your existing models and use those forms to reate and update data.
- Django comes with a secure authentication system, which makes it easier to create sites that allow users to create accounts and safely log in/out.
- It has an automatic admin interface. Reads metadata in your models to provide a powerful and production-ready interface
- It offers support for translating text into different languages and locale-specific formatting of dates, times etc.
- Provides security against:
  - Clickjacking
  - Cross-site scripting
  - Cross Site Request Forgery (CSRF)
  - SQL injection
  - Remote code execution

### How Django Works Behind The Scenes

- 



### Sources

[Getting Started with Django](https://www.djangoproject.com/start/)<br>
[How Django Works Behind The Scenes](https://wsvincent.com/how-django-works-behind-the-scenes/)<br>
[Django introduction](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Introduction)<br>
[Writing your first Django app, part 1](https://docs.djangoproject.com/en/4.1/intro/tutorial01/)<br>
[Writing your first Django app, part 2](https://docs.djangoproject.com/en/4.1/intro/tutorial02/)<br>