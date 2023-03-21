todo project
========

About
-----

The main aim of this project is working with databases and creating websites


Author: Vitaliy Pavlovich <vitalliypavlovich@mail.ru>

Source link: https://github.com/vitaliypavlovich/todo

Project structure
-----

todo/ - project root folder, repository

manage.py - Django app

.venv/ - virtual environment

Setup dev environment
---------------------
1. Сreate a virtual environment

2. PostgreSQL server setup

      $ sudo apt install python3-virtualenv

      $ virtualenv -p python3 --prompt=todo .venv/
      
      $ python3 -m venv --prompt=todo .venv/
            
      $ source .venv/bin/activate


      $ sudo su postgres

      $ psql

      $ CREATE USER 'user' WITH PASSWORD 'password' CREATEDB;
      
      $ CREATE DATABASE todo OWNER 'owner';

Build and run app in dev mode
-----------------------------


1. Creating base tables in the database
      
      $ cd projects/todo/
      
      $ python manage.py migrate

2. Creating a system user
      
      $ python manage.py createsuperuser

3. Starting a local server
      
      $ python manage.py runserver
      
Production setup
----------------

1. Install django

2. Install PostgreSQL
