# learning_log
The Learning Log home page will describe the
site and invite users to either register or log in. 
Once logged in, a user can create new topics, add 
new entries, and read and edit existing entries.

* learning_log$ python -m venv venv `Creating a Virtual Environment`
* learning_log$ source venv/Scripts/activate `Activating the Virtual Environment for windows`
* (venv)learning_log$ pip install django `Installing Django`
* (venv)learning_log$ django-admin startproject learning_log . `Creating a Project in Django`
* (venv)learning_log$ python manage.py migrate `Creating the Database`
* (venv)learning_log$ python manage.py runserver `Starting Server at http://127.0.0.1:8000/`
* (venv)learning_log$ deactivate `Deactivate the Virtual Environment`
