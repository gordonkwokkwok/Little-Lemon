# Little Lemon

## Introduction


## Prerequisite
Creating a virtual environment is recommended for projects, and either venv or conda can be used based on personal preference. After creating the virtual environment, it is necessary to activate it before installing any required libraries, such as the Django framework.

### Tool
```
Visual Studio Code (Version: 1.75.1)
Git (Version: 2.23.0)
Conda (Version: 22.9.0)
Python (Version: 3.9.6)
pip (Version: 23.0.1)
MySQL Connect
```

### Library
```
Use "pip install " command to install the following libraries:
pip install Django (Version: 4.1)
pip install 
```

## Command

### Activate Virtual Environment
```
conda activate djangoEnv
```

### Start the project
```
django-admin startproject littlelemon
cd littlelemon
python3 manage.py startapp reservation
(Add reservation in setting.py file in the installed apps list)

```

### Run development server
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver

<!-- ## Database Schema
The POS data will be loaded and stored in a MySQL database table:
- xxx -->

# Reminder


## Contributers
- [Gordon Kwok](https://www.linkedin.com/in/gordonkwokch/)