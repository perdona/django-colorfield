=================
django-colorfield
=================

Simple colorfield for django (optimized for carlosroberto)

Installation
============

Instaling django-colorfield::

    pip install -e git://github.com/renecarvalho/django-colorfield.git#egg=colorfield

Add `colorfield` to your `INSTALLED_APPS`, example::

    INSTALLED_APPS = (
        'colorfield',
    )

Then in your models, you can use it like this::

    from django.db import models
    from colorfield.fields import ColorField


    class Show(ExtendedModel):
        title = models.CharField(u'Title', max_length=250)
        color = ColorField(default='ffffff')


    
