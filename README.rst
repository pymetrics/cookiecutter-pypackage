======================
Cookiecutter PyPackage
======================

.. image:: https://app.travis-ci.com/pymetrics/cookiecutter-python-library.svg?branch=master
    :target: https://app.travis-ci.com/github/pymetrics/cookiecutter-python-library
    :alt: Build Status

.. image:: https://readthedocs.org/projects/cookiecutter-python-library/badge/?version=latest
    :target: https://cookiecutter-python-library.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status

Cookiecutter_ template for a Python package.

* GitHub repo: https://github.com/pymetrics/cookiecutter-python-library/
* Documentation: https://cookiecutter-python-library.readthedocs.io/
* Free software: BSD license

Features
--------

* Testing setup with ``unittest`` and ``python setup.py test`` or ``pytest``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 3.7, 3.8, and 3.9,
  with optional support for Python 3.6
* Sphinx_ docs: Documentation ready for generation with, for example, `Read the Docs`_
* bump2version_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click or argparse (optional)

.. _Cookiecutter: https://github.com/cookiecutter/cookiecutter


Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/pymetrics/cookiecutter-python-library.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``)
* Register_ your project with PyPI.
  * Run ``twine upload dist/*``.
* For an open source project, `create a PyPI API token`_, with scope limited to the project,
  for publishing.
* Set PyPI credentials in TravisCI environment variables ``PYPI_USERNAME`` and ``PYPI_PASSWORD``.
  * If using an API token, set ``PYPI_USERNAME`` to ``__token__``.
* Add the repo to your `Read the Docs`_ account + turn on the Read the Docs service hook.
* Release your package by pushing a new tag to master.
* Add a ``requirements.txt`` file that specifies the packages you will need for
  your project and their versions. For more info see the `pip docs for requirements files`_.

.. _`create a PyPI API token`: https://pypi.org/manage/account/#api-tokens
.. _`pip docs for requirements files`: https://pip.pypa.io/en/stable/user_guide/#requirements-files
.. _Register: https://packaging.python.org/tutorials/packaging-projects/#uploading-the-distribution-archives

For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html


Credits
~~~~~~~

Forked from `@audryr's cookiecutter-pypackage`_.

.. _`@audryr's cookiecutter-pypackage`: https://github.com/audreyfeldroy/cookiecutter-pypackage


.. _Travis-CI: http://travis-ci.com/
.. _Tox: http://testrun.org/tox/
.. _Sphinx: http://sphinx-doc.org/
.. _Read the Docs: https://readthedocs.io/
.. _bump2version: https://github.com/c4urself/bump2version
.. _Punch: https://github.com/lgiordani/punch
.. _Poetry: https://python-poetry.org/
.. _PyPi: https://pypi.python.org/pypi
.. _Mkdocs: https://pypi.org/project/mkdocs/
.. _Pre-commit: https://pre-commit.com/
.. _Black: https://black.readthedocs.io/en/stable/
.. _Mypy: https://mypy.readthedocs.io/en/stable/
