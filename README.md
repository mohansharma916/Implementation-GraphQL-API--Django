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

