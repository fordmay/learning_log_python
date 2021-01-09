# learning_log
The Learning Log home page will describe the
site and invite users to either register or log in. 
Once logged in, a user can create new topics, add 
new entries, and read and edit existing entries.
---
* learning_log$ python -m venv venv `Creat a Virtual Environment`
* learning_log$ source venv/Scripts/activate `Activate the Virtual Environment on Windows`
* (venv)learning_log$ pip install django `Install Django`
* (venv)learning_log$ django-admin startproject learning_log . `Creat a Project in Django`
* (venv)learning_log$ python manage.py migrate `Creat the Database`
* (venv)learning_log$ python manage.py runserver `Start Server at http://127.0.0.1:8000/`
* CTRL+C - `Close Server`
* (venv)learning_log$ deactivate `Deactivate the Virtual Environment`
---
The Django Shell:
* (venv)learning_log$ python manage.py shell `Start Shell session`
* &gt;&gt;&gt; from learning_logs.models import Topic `Import the model Topic`
* &gt;&gt;&gt; Topic.objects.all() `Get all the instances of the model Topic`

1. &gt;&gt;&gt; topics = Topic.objects.all()
2. &gt;&gt;&gt; for topic in topics: `Loop over a Queryset`
3. ... print(topic.id, topic) `Show the ID that’s been assigned to each topic object`

- &gt;&gt;&gt; topic = Topic.objects.get(id=1)
- &gt;&gt;&gt; topic.text `Show at the text for ID 1`
- &gt;&gt;&gt; topic.date_added `Show date added values for ID 1`
- &gt;&gt;&gt; topic.entry_set.all() `Get every Entry related to ID 1`

+ __CTRL-Z__ and then press __ENTER__ `Close a Shell session on
Windows`