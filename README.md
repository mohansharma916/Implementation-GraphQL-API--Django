# Implementing-GraphQL-with-Django

Before Going Forward First Lets Understand about GraphQL

<strong> 1. What is GraphQL? </strong>

GraphQL is a query language and server-side runtime for application programming interfaces (APIs) that prioritizes giving clients exactly the data they request and no more. GraphQL is designed to make APIs fast, flexible, and developer-friendly.


In This Repositry I Have  Implemented GraphQL with Django , It will be a Fun to do that Lets Begin ................


# Install and Setup Django & GraphQL

First Create a Python Virtual Environment and Activating It in the desired Working Directory.

open your Working Directory in Terminal

```
$ python3 -m venv env

```

Activating the Virtual Environment 

```
$ source env/bin/activate

```
After the Virtual Environemnt is Created and Activated , Lets Install Django which are the necessary Python Libraries.

Installl Django Version 3. Django version 4 is not compataible with Graphene( Required Library for Implementing GraphQL)

```
$ pip install Django==3.1.14

```

After Installing the necessary requirements let's Create A Django Project (quickstart) and app (users)


```
(env)$ django-admin startproject quickstart
(env)$ cd quickstart

```

```

(env) $ python manage.py startapp users

```

After the App is created , Lets Register the app by adding the path to the ***quickstart/settings.py***.

```
#quickstart/settings.py

INSTALLED_APPS=[
      ......
      'users'
              ]
```

Now Lets Check the App is running or not by Using Django runserver Command

```
(env) $ python manage.py runserver

```

if everything works as Shown above, and if we  go http://127.0.0.1:8000/ in the browser we should see the following success message.

![Screenshot 2022-10-05 at 9 22 17 PM](https://user-images.githubusercontent.com/77909856/194105352-8d5c3d10-11c9-448b-acee-f1a96a41277b.png)


# Set up Custom user Model

```
#users/models.py

from django.contrib.auth.models import AbstractUser

class CustomUser(AbstractUser):
      
    email = models.EmailField(blank=False, max_length=254, verbose_name="email address")

    USERNAME_FIELD = "username"   # e.g: "username", "email"
    EMAIL_FIELD = "email"         # e.g: "email", "primary_email"


```

Add it to the Settings:

```
 #quickstart/settings.py

AUTH_USER_MODEL='users.CustomUser'
 
```

Then, Migrate

```
(env) $ python manage.py migrate

```



# Setup Graphene and GraphQL JWT

<strong> 2. What is Graphene-Django ?</strong>
Graphene-Django "make it easy to add GraphQL functionality to your Django project".


<strong>3. What is Django-GraphQL-JWT ?</strong>

Django-GraphQL-JWT is the easiest way to add JSON Web token authentication for Django with GraphQL.





