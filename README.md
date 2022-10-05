# Implementing-GraphQL-with-Django

Before Going Forward First Lets Understand about GraphQL

<strong> 1. What is GraphQL? </strong>

GraphQL is a query language and server-side runtime for application programming interfaces (APIs) that prioritizes giving clients exactly the data they request and no more. GraphQL is designed to make APIs fast, flexible, and developer-friendly.


In This Repositry I Have  Implemented GraphQL with Django ,
Lets Begin ................

<strong> 2. What is Graphene-Django ?</strong>

Graphene-Django "make it easy to add GraphQL functionality to your Django project".


<strong>3. What is Django-GraphQL-JWT ?</strong>

Django-GraphQL-JWT is the easiest way to add JSON Web token authentication for Django with GraphQL.

#How to Use It.


1.Clone This Repository 

open Terminal/Command Prompt

go to Desired Working Directory 

```
$ git clone https://github.com/mohansharma916/Implementation-GraphQL-API--Django.git
```

then Go to inside the Folder (in your Local System)

```
$ cd Implementation-GraphQL-API--Django

```

Create A Virtual Environment

```
$ python3 -m venv env

```

Activate the Virtual Environment

```
$ source env/bin/activate

```
once the environment is activate

```
(env) $ cd quickstart

```
now Lets Install all The Requirements

```
(env) $ pip install -r requirements.txt

```
Above Mentioned Command will install all the Dependencises still Maybe you face some error 
to solve these dependencise you can use below mentioned command 

```
>$pip install Django==3.1.14
>$pip install graphene_django
>$pip install django-graphql-jwt
>$pip install django-graphql-auth

```


after this Migrate your Models

```
 (env)$ python manage.py migrate
 
 Operations to perform:
  Apply all migrations: admin, auth, contenttypes, graphql_auth, refresh_token, sessions, users
Running migrations:
  Applying users.0002_auto_20221005_1455... OK
  
  (env) python manage.py makemigrations
  
   No changes detected
   
   (env) python manage.py runserver
   Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
October 05, 2022 - 18:04:05
Django version 3.1.14, using settings 'quickstart.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C


```
  
  


```
