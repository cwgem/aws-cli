============
Introduction
============

This is a description of the overall code layout for ``aws-cli``. The intention
is to make it easier for those who wish to contribute, or are simply curious as
to how the code works, understand the purpose of various files and directories.

==================
Toplevel Structure
==================

Setup Related Files
-------------------

The following are utilized for distribution and installation purposes:

- ``setup.py``: The distutils setup script
- ``setup.cfg``: Configuration file for the ``setup.py`` file
- ``MANIFEST.in``: For packaging purposes, provides a list of non-python
  related files to include
- ``requirements*.txt``: These files are mainly used with `pip`_ to provide a
  list of packages to install for various parts of the code base to work

Testing Related Files
---------------------

The following are utilized for test suite purposes:

- ``tests``: Folder containing the test suites
- ``tox.ini``: Test environment automation configuration for `tox`_
- ``.travis.yml``: Continuous integration configuration for `Travis CI`_
- ``.coveragerc``: Code coverage configuration for `Coverage.py`_
- ``scripts``: This folder contains a number of testing related files, including
  benchmarks for some S3 operations

Documentation Related Files
---------------------------

The following are related to or contain documentation:

- ``ARCHITECTURE.rst``: This file, describing the code layout
- ``CHANGELOG.rst``: A list of changes to the project over time
- ``CONTRIBUTING.rst``: Outlines how to contribute to the project
- ``README.rst``: A general overview of the project
- ``LICENSE.txt``: A copy of the Apache 2.0 license for this project
- ``.changes``: Similar to ``CHANGELOG.rst`` but in JSON formatted files
- ``doc``: `Sphinx`_ related documentation files

Module Related Files
--------------------

The following are related to the overall functionality of `aws-cli` in terms
of runtime usage:

- ``awscli``: The core code for ``aws-cli``
- ``bin``: The ``aws-cli`` binary files, acting as a frontend for the code

.. _tox: https://github.com/tox-dev/tox
.. _Travis CI: https://travis-ci.org/
.. _Coverage.py: http://coverage.readthedocs.io/en/latest/config.html
.. _Sphinx: http://www.sphinx-doc.org/en/stable/
.. _pip: https://pypi.python.org/pypi/pip
