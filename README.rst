========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - tests
      - | |travis| |appveyor| |requires|
        | |codecov|
    * - package
      - | |version| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|

.. |travis| image:: https://api.travis-ci.com/russarmst/python-phctl.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.com/github/russarmst/python-phctl

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/russarmst/python-phctl?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/russarmst/python-phctl

.. |requires| image:: https://requires.io/github/russarmst/python-phctl/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/russarmst/python-phctl/requirements/?branch=master

.. |codecov| image:: https://codecov.io/gh/russarmst/python-phctl/branch/master/graphs/badge.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/russarmst/python-phctl

.. |version| image:: https://img.shields.io/pypi/v/phctl.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/phctl

.. |wheel| image:: https://img.shields.io/pypi/wheel/phctl.svg
    :alt: PyPI Wheel
    :target: https://pypi.org/project/phctl

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/phctl.svg
    :alt: Supported versions
    :target: https://pypi.org/project/phctl

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/phctl.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/phctl

.. |commits-since| image:: https://img.shields.io/github/commits-since/russarmst/python-phctl/v0.0.1.svg
    :alt: Commits since latest release
    :target: https://github.com/russarmst/python-phctl/compare/v0.0.1...master



.. end-badges

A Python package to control Pihole.

* Free software: MIT license

Installation
============

::

    pip install phctl

You can also install the in-development version with::

    pip install https://github.com/russarmst/python-phctl/archive/master.zip


Documentation
=============


To use the project:

.. code-block:: python

    import phctl
    phctl.longest()


Development
===========

To run all the tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox
