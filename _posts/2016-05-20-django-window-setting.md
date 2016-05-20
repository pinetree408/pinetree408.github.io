---
layout: post
maintitle: Django Window Settings
subtitle: Start django with window env
---

## What issuse

I want to use window for django server

## How to study

1. Install python

Python 2.7 with msi for windows(x64)

2. Setting python to PATH

Computer > property > advance > path

```
C:\Python27\;C:\Python27\Scripts\
```

3. Install virtualenv in CMD

```
pip install virtualenv
```

4. Run Virtualenv

```
<virtualenv_name>\Scripts\activate
```

5. Install django with pip

```
pip install django==1.8
```

6. Make Project

```
python C:\Path\To\<virtualenv_name>\Scripts\django-admin.py startproject <project_name>
```

7. Now Runserver!

```
python manage.py runserver
```
