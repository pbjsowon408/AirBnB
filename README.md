# AirBnB
Clone Project


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

