# Django Models

## Django Definition

Django is a **Web framework written in Python**. A Web framework is software that supports the development of dynamic Web sites, applications, and services. It provides a set of tools and functionalities that solves many common problems associated with Web development, such as security features, database access, sessions, template processing, URL routing, internationalization, localization, and much more.

Using a Web framework, such as Django, enables us to develop secure and reliable Web applications very quickly in a standardized way, without having to reinvent the wheel.

- The **initial project structure** is composed of five files:

  - manage.py: a shortcut to use the django-admin command-line utility. It’s used to run management commands related to our project. We will use it to run the development server, run tests, create migrations, and much more.

  - **init**.py: this empty file tells Python that this folder is a Python package.

  - settings.py: this file contains all the project’s configurations. We will refer to this file all the time!

  - urls.py: this file is responsible for mapping the routes and paths in our project. For example, if you want to show something in the URL /about/, you have to map it here first.

  - wsgi.py: this file is a simple gateway interface used for deployment. You don’t have to bother about it.

- The **app project structure** is composed of six files:

  - migrations/: here Django store some files to keep track of the changes you create in the models.py file, so as to keep the database and the models.py synchronized.

  - admin.py: this is a configuration file for a built-in Django app called Django Admin.

  - apps.py: this is a configuration file of the app itself.

  - models.py: here is where we define the entities of our Web application. The models are translated automatically by Django into database tables.

  - tests.py: this file is used to write unit tests for the app.

  - views.py: this is the file where we handle the request/response cycle of our Web application.

&nbsp;

## Using models

Django web applications access and manage data through Python objects referred to as models. Models define **the structure of stored data**, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc.

When designing your models it makes sense to have separate models for every "object" (a group of related information).

Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods, and metadata.

Minimally, in every model, you should define the standard Python class method **str**() to return a human-readable string for each object.

Once you've defined your model classes you can use them to create, update, or delete records, and run queries to get all records or particular subsets of records.

&nbsp;

## Django admin site

The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data. The admin application can also be useful for managing data in production, depending on the type of website. The Django project recommends it only for internal data management

In order to log into the admin site, we need a user account with Staff status enabled. In order to view and create records we also need this user to have permissions to manage all our objects. You can create a "superuser" account that has full access to the site and all needed permissions using manage.py.
