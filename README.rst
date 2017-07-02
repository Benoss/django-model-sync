=============================
Django Model Sync
=============================

.. image:: https://badge.fury.io/py/django-model-sync.svg
    :target: https://badge.fury.io/py/django-model-sync

.. image:: https://travis-ci.org/Benoss/django-model-sync.svg?branch=master
    :target: https://travis-ci.org/Benoss/django-model-sync

.. image:: https://codecov.io/gh/Benoss/django-model-sync/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/Benoss/django-model-sync

Django Model Sync allow you to sync your local models with a distant install of Django over http. With optional encryption and anonymization hooks

Documentation
-------------

The full documentation is at https://django-model-sync.readthedocs.io.

Quickstart
----------

Install Django Model Sync::

    pip install django-model-sync

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'django_model_sync.apps.DjangoModelSyncConfig',
        ...
    )

Add Django Model Sync's URL patterns:

.. code-block:: python

    from django_model_sync import urls as django_model_sync_urls


    urlpatterns = [
        ...
        url(r'^', include(django_model_sync_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
