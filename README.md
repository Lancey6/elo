ELO
===
Electronic Ladder Organizer

Pronounced "E. L. O." as it's an actual acronym, unlike Elo.

Things Used
-----
* [Django 1.7.4](https://www.djangoproject.com/)
* [python-openid 2.2.5](https://github.com/openid/python-openid)
* [django-openid-auth 0.5](https://pypi.python.org/pypi/django-openid-auth/)*
* [Pillow 2.7.0](https://github.com/python-pillow/Pillow)

Setup/Notes
--
**django-openid-auth**: Due to a change in django 1.6, urls.py in django-openid-auth needs to be updated:

`django.conf.urls.defaults` should become `from django.conf.urls import patterns, url, include`

**dbase/**: Create this (empty) folder in the base directory.

**elo/settings.py**: Add a secret key and change the `CSRF_COOKIE_DOMAIN` to `127.0.0.1`