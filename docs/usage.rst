=====
Usage
=====

To use Django Model Sync in a project, add it to your `INSTALLED_APPS`:

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
