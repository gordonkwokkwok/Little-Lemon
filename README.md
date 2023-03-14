# Little Lemon

## Introduction
This is a capstone project in Django, specifically building an API for the Little Lemon restaurant using the Django REST Framework. The Capstone project demonstrates multiple skills by solving an authentic real-world problems. For example, 

- Set up the Github repository
- Set up the Django project
- Set up the static and templates routes
- Set up the MySQL connection
- Set up the models
- Querying the stored procedures
- Set up the menu API
- Set up the table booking API
- Work with user authentication (remote user, session, token-based)
- Add the registration, login, logout functionality page (Djoser)
- Secure the table booking API
- Adding unit tests
- Testing the API using Insomnia


# Prerequisite
Creating a virtual environment is recommended for projects, and either venv or conda can be used based on personal preference. After creating the virtual environment, it is necessary to activate it before installing any required libraries, such as the Django framework and Django REST framework.

## Tool
```
Visual Studio Code (Version: 1.75.1)
Git (Version: 2.23.0)
Conda (Version: 22.9.0)
Python (Version: 3.9.6)
pip (Version: 23.0.1)
MySQL(Version: 8.0.32 for macos13.0 on x86_64 (Homebrew))
Insomnia REST client
```

## Library / Framework
```
Use "pip3 install " command to install the following libraries:
pip3 install Django (Version: 4.1)
pip3 install virtualenv (or use conda virtual environment)
pip3 install mysqlclient 
pip3 install djangorestframework (Add 'rest_framework' in setting.py file in the installed apps list)
pip3 install djoser (Add 'djoser' in setting.py file in the installed apps list, and ensure that it is placed after the 'rest_framework' app in the list.)
```

# Command to create a Django project and an app:
```
conda activate djangoEnv (activate the conda virtual environment)
django-admin startproject littlelemon
cd littlelemon
python3 manage.py startapp reservation (Add 'reservation' in setting.py file in the installed apps list)
cd ..
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py createsuperuser (Username: admin, Password: 123456)
python3 manage.py runserver
```

# APIs
## ```restaurant/menu```

Allow all authenticated users to view the menu items.
Only admin user could post new item.

Fields needed to post:

>**Title**: str

>**Price**: decimal

>**Inventory**: int

## ```restaurant/menu/<int:pk>```

Allow all authenticated users to view single menu item.

Only admin user could update or delete single item.

## ```restaurant/book```

Allow authenticated users to post new booking, please use the same username of the user as the name of booking.

User could obtain all the books that has the same book name with the current username.

Fields needed to post:

>**name**: str, the same as username

>**guest_number**: (opt.) int, default = 1

>**date**: date, in the form of "YYYY-MM-DD"

>**comment**: (opt.) text

## ```restaurant/book/<int:pk>```
Only admin user could view or delete single book

# Current users
##  Superuser/admin:

>**Username**: admin
>**Password**: 123456

##  Customer:

>**Username**: testinguser1
>**Password**: lemon@123!

>**Username**: testinguser2
>**Password**: lemon@123!

>**Username**: testing1
>**Password**: fewfewfvrgre435435

# Contributer
- [Gordon Kwok](https://www.linkedin.com/in/gordonkwokch/)