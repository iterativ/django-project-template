========================
django-twoscoops-project
========================

Newer versions
==============

Please take a look at 

https://github.com/iterativ/cookiecutter-simple-django

or

https://github.com/iterativ/cookiecutter-simple-django-spa

which does the same




A project template for Django 1.5.

To use this project follow these steps:

#. Create your working environment
#. Install Django
#. Create the new project using the django-two-scoops template
#. Install additional dependencies
#. Use the Django admin to create the project

*note: these instructions show creation of a project called "icecream".  You
should replace this name with the actual name of your project.*

Creating your project
=====================

To create a new Django project called '**icecream**' using
django-project-template, run the following command:

    $ django-admin.py startproject --template=https://github.com/iterativ/django-project-template/zipball/master --extension=py,rst,html,rb,pp,json --name=Vagrantfile icecream

Create virtual env

    $ virtualenv --no-site-packages icecream-env

Installation of Dependencies
============================

Depending on where you are installing dependencies:

In development::

    $ pip install -r requirements/local.txt

For production::

    $ pip install -r requirements.txt

*note: We install production requirements this way because many Platforms as a
Services expect a requirements.txt file in the root of projects.*

Initialize Database
===================

Create all tables an load a admin user (admin, test)

    $ python manage.py resetload
