.. image:: https://travis-ci.org/shuup/shuup.svg?branch=master
    :target: https://travis-ci.org/shuup/shuup
.. image:: https://coveralls.io/repos/github/shuup/shuup/badge.svg?branch=master
   :target: https://coveralls.io/github/shuup/shuup?branch=master
.. image:: https://img.shields.io/pypi/v/shuup.svg
   :alt: PyPI
   :target: https://github.com/shuup/shuup
.. image:: https://snyk.io/test/github/shuup/shuup/badge.svg
   :alt: Known Vulnerabilities
   :target: https://snyk.io/test/github/shuup/shuup

Slump


Docker quick start
------------------

Fastest way to get Slump up and running is to use `Docker <https://www.docker.com>`_.

1. Run:

   .. code-block:: shell

      docker-compose up

2. Open `localhost:8000/sa <http://localhost:8000/sa>`_ in a browser,
   log in with username: ``admin`` password: ``admin``

Full Slump installation guide
-----------------------------

See `Getting Started
<http://shuup.readthedocs.io/en/latest/howto/getting_started.html>`__.

For simple project example see our `Django-project template <https://github.com/shuup/shuup-project-template>`__.

Getting Started with Slumpdevelopment
--------------------------------------

See `Getting Started with Slump Development
<http://shuup.readthedocs.io/en/latest/howto/getting_started_dev.html>`__.


Documentation
-------------

Documentation is built with `Sphinx <http://sphinx-doc.org/>`__.

Issue the following commands to build the documentation:

.. code:: sh

    pip install -r requirements-doc.txt
    cd doc && make html

To update the API documentation rst files, e.g. after adding new
modules, use command:

.. code:: sh

    ./generate_apidoc.py

Roadmap
-------

v3 (Q4 2021)
###############

* Initial Django 3.x support
* Latest Jinja support
* Deprecate theme folders under Shuup front which are used to override
  individual macros in macro folders. This does not work well with latest
  Jinja and adds extra complexity.

v4 (Q1 2022)
#############

* Move Shuup front, xtheme and theming features to own addons. This so that
  projects not ready for updating theme or front can still get latest Shuup.
* Introduce new default theme and overhaul templates structure to be more
  simple (likely Bootstrap 5 will be used).
* Bump admin Bootstrap version to match with the new front
* Move various other not essential apps in this repository to addons for
  better version management.

Additional Material
-------------------

* `Django-project template <https://github.com/shuup/shuup-project-template>`__. Django-project template.
* `Provides system <https://shuup.readthedocs.io/en/latest/ref/provides.html>`__.
* `Core settings <https://shuup.readthedocs.io/en/latest/api/shuup.core.html#module-shuup.core.settings>`__.
* `Front settings <https://shuup.readthedocs.io/en/latest/api/shuup.front.html#module-shuup.front.settings>`__.
* `Admin settings <https://shuup.readthedocs.io/en/latest/api/shuup.admin.html#module-shuup.admin.settings>`__.
* `Extending Shuup <https://shuup.readthedocs.io/en/latest/#extending-shuup>`__.


Admin Preview
-------------

.. image:: _static/admin_shop_product.png
    :target: _static/admin_shop_product.png
    :height: 300px

.. image:: _static/admin_order_detail.png
    :target: _static/admin_order_detail.png
    :height: 300px
