******************
djangocms-lab-tags
******************

``djangocms-lab-tags`` is a Django app for consolidating content tagged with ``django-taggit`` tags within a Django site with django CMS-specific features.

Source code is available on GitHub at `mfcovington/djangocms-lab-tags <https://github.com/mfcovington/djangocms-lab-tags>`_. Information about ``django-taggit`` is available on `GitHub <https://github.com/alex/django-taggit>`_ and `Read the Docs <http://django-taggit.readthedocs.org/en/latest/index.html>`_.

.. contents:: :local:


.. Installation
.. ============

.. **PyPI**

.. .. code-block:: sh

..     pip install djangocms-lab-tags

.. **GitHub**

.. .. code-block:: sh

..     pip install https://github.com/mfcovington/djangocms-lab-tags/releases/download/0.1.4-dev1/djangocms-lab-tags-0.1.4-dev1.tar.gz


Configuration
=============

Do the following in ``settings.py``:

- Add ``cms_lab_tags`` and its dependencies to ``INSTALLED_APPS``:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'taggit',
        'cms_lab_tags',
    )


.. Migrations
.. ==========

.. Create and perform ``cms_lab_tags`` migrations:

.. .. code-block:: sh

..     python manage.py makemigrations cms_lab_tags
..     python manage.py migrate


Usage
=====

- Start the development server:

.. code-block:: sh

    python manage.py runserver

- Visit: ``http://127.0.0.1:8000/``
- Create a CMS page and then:

  - Attach the ``Tags App`` under ``Advanced Settings`` for the page, **OR**
  - Insert the ``Tag Plugin`` into a placeholder field.


*Version 0.0.0*
