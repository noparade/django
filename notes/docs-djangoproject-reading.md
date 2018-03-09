
- manage.py : A command-line utility that lets you interact with this Django project in various ways
- __init__.py : An empty file that tells Python that this directory should be considered a Python package


- deal with configuring a production server – such as Apache

 __don’t use this server in anything resembling a production environment. 
 It’s intended only for use while developing. (We’re in the business of making Web frameworks, not Web servers.)__



__If you want to change the server’s IP, pass it along with the port. For example, to listen on all available public IPs (which is useful if you are running Vagrant or want to show off your work on other computers on the network), use:__
` python manage.py runserver 0:8000`

A __view__ function, or view for short, is simply a Python function that takes a Web request and returns a Web response. 

`urls.py` in app; index
`urls.py` in project: link to root url

The __path()__ function is passed four arguments, two required: route and view

Patterns don’t search GET and POST parameters, or the domain name. For example, in a request to https://www.example.com/myapp/, the URLconf will look for myapp/. In a request to https://www.example.com/myapp/?page=3, the URLconf will also look for myapp/.

`django.db.backends.postgresql`

- `django-admin startproject mysite` # start a new project
- `python manage.py runserver`
- `python manage.py runserver 8080`
- `python manage.py startapp polls` # # start a new app
