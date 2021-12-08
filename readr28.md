# Django Best Practices: Custom User Model

# Readings: Django Custom User  :
* Django ships with a **built-in** User model for authentication .
* The official Django documentation highly recommends using a custom user model. 
##### Setup
* To start, create a new Django project from the command line. We need to do several things:
1. create and navigate into a dedicated directory called accounts for our code
2. install Django
3. make a new Django project called config.
4. make a new app accounts
5. start the local web server
* ** Note that we did not run migrate to configure our database. It's important to wait until after we've created our new custom user model before doing so.

* There are two modern ways to create a custom user model in Django: **AbstractUser** and **AbstractBaseUser**. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work.
* AbstractUser actually subclasses AbstractBaseUser but provides more default configuration.

```
$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver
```

## AbstractUser vs AbstractBaseUser


- Custom User Model Creating our initial custom user model requires four steps:

    - update config/settings.py
    - create a new CustomUser model
    - create new UserCreation and UserChangeForm
    - update the admin
    - In settings.py we’ll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model.



## Superuser

- It’s helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.

- Now that our custom user model is configured you can easily and at any time add additional fields to it. See the Django docs for further instructions.

- DjangoX, which is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.
