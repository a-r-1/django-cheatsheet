# django-cheatsheet
A compilation of useful code snippets to create, set up, and develop a Django project.

Code Of Conduct:
- TBA...

Styling Guidelines:
- TBA...

Requirements:

- Python
- Pip
- Django

## Table of Contents

- [Installing Django](#install_django)
- [Creating a project](#create_project)
- [Starting the Server](#start_server)
- [Django Models](#models)
- [Django Views](#views)
- [URL Patterns](#url_patterns)


<a name="install_django"></a>

## Installing Django

<pre><code>
pip install django

</code></pre>


<a name="create_project"></a>

## Creating a project

<pre><code>
django-admin startproject project-name

</code></pre>

<a name="start_server"></a>

## Starting the Server

<pre><code>
python manage.py runserver

</code></pre>


<a name="models"></a>

## Django Models

<pre><code>
from django.db import models

class ModelName(models.Model):
ModelName_id = models.AutoField

</code></pre>

<a name="views"></a>

## Django Views

- Views.py

<pre><code>
from django.http import HttpResponse

def index(request):
return HttpResponse("cheatsheet")

</code></pre>

<a name="url_patterns"></a>

## URL Patterns

<pre><code>
from django.contrib import admin
from django.urls import path
from . import views

urlpatterns = [
path('admin/', admin.site.urls),
path('', views.index, name='index'),
path('about/', views.about, name='about'),
path('contact/', views.contact, name='contact'),
]

</code></pre>

<br>
<a>Here (TBA) </a>
