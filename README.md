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
