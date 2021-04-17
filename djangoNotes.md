<h3> Creating a new project in Django </h3>

from the tutorial : https://docs.djangoproject.com/en/3.1/intro/tutorial01/

```django-admin startproject mysite```

<h3> Project structure </h3>
  
 ```
 mysite/
    manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
 ```
 <h3> Running code </h3>
 
 ```
 cd mysite
 python manage.py runserver
 
 ```
 <h3> Creating an app inside project </h3>
 
 ```python manage.py startapp polls```
 
 <h3> Directory structure of app </h3>
 
 ```
 polls/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
 ```
 
