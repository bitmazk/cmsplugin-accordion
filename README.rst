CMSPlugin Accordion
============

django-cms plugin that allow to create accordions on the frontend.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install cmsplugin-accordion

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/cmsplugin-accordion.git#egg=cmsplugin_accordion

TODO: Describe further installation steps (edit / remove the examples below):

Add ``cmsplugin_accordion`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'cmsplugin_accordion',
    )

Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate cmsplugin_accordion


Usage
-----

1. Create a new ``Accordion`` instance via the Django admin.
2. Create a few ``AccordionRow`` instances via the Django admin that belong
   to the Accordion instance you created before.
3. Go to one of your CMS pages and add the ``Accordion Plugin``
4. Edit the ``cmsplugin_accordion/accordion_plugin.html`` template to your
   liking.

That's it. You should now be able to embed accordions into your placeholders.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 cmsplugin-accordion
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
