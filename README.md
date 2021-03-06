# AirBnB
Clone Project
-----------------------------------------------------------
Front-End   : HTML, CSS, VanillaJS, Tailwind CSS, GULP
Back-End    : Python, Django, AWS, Heroku (for distribution)
Environment : Visual Studio Code, Git

<Features>
User Registration / Profile
Social Authentication
Superuser Admin Panel
Host Admin Panel
Guest Dashboard
2-way Review System
Bookin and Reservation System
Direct Messaging
Room CRUD
Notification Email
Ajax Searching
  
<Technologies>
Python
Django
HTML5
Tailwind CSS
GULP
ES6
Google Maps
Twilio
Mailgun
Boto
Heroku & AWS S3
  
--------------------------------------
*Tip how to import
1.import Python package
2.import everything related in Django
3.import Third-Party packages
4.import custom packages

-----------------------------------------
(For now, I am just documenting every core steps for building AirBnB clone project while coding as well.)
//Make bubble

pip3 install --user pipenv

pipenv --three

//Go inside the bubble

pipenv shell  // always put this code in cmd when reboot

pipenv install Django==2.2.5 (the same as npm of package.json)

//https://github.com/github/gitignore/blob/master/Python.gitignore

git init
git remote add origin https://github.com/pbjsowon408/AirBnB
git add .
type nul > .gitignore (touch .gitignore)

django-admin startproject config // rename first config folder as Aconfig, drag config folder and files that were inside to outside. Remove Aconfig folder

pipenv install flake8 --dev
pipenv install black --dev --pre

--------------------------------------------
python manage.py runserver // running the server. Always have to runserver to run Django server

python manage.py migrate // when shape of the data changes, create, apply , and update migration. Which will synchronize with the DB

python manage.py createsuperuser // create superuser

---------------------------------------------

django-admin startapp (application name) // application name should be plural. ex)room X   |   rooms O

django-admin startapp rooms // search rooms
django-admin startapp users // log-in log-out  (such as login as facbook)
django-admin startapp reviews // leave a review
django-admin startapp conversations // Talk to the people
django-admin startapp lists // make a list of the liked rooms
django-admin startapp reservations // view reservations

---------------------------------------------------------

pipenv install Pillow  // to use image file in db


*important (in config/settings)
DJANGO_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",
]

PROJECT_APPS = [
    "users.apps.UsersConfig",
]

INSTALLED_APPS = DJANGO_APPS + PROJECT_APPS

AUTH_USER_MODEL = "users.User"
