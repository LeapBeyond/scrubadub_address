
.. NOTES FOR CREATING A RELEASE:
..
..   * bump the version number in scrubadub_stanford/__init__.py
..   * update docs/changelog.rst
..   * git push
..   * create a release https://github.com/LeapBeyond/scrubadub_address/releases
..      * This should trigger a github action to upload to pypi
..      * ReadTheDocs.io should see any changes and also rebuild the docs


*****************
scrubadub_address
*****************

``scrubadub`` removes personally identifiable information from text.
``scrubadub_address`` is an extension that uses ``pyap`` and ``libpostal`` to remove addresses from text.

This package contains one extra detector:

* ``scrubadub_address.detectors.AddressDetector`` - A detector that finds British, American and Canadian addresses.

For more information on how to use this package see the
`scrubadub address documentation <https://scrubadub.readthedocs.io/en/develop/addresses.html>`_
and the `scrubadub repository <https://github.com/LeapBeyond/scrubadub>`_.


.. image:: https://img.shields.io/github/workflow/status/LeapBeyond/scrubadub_address/Python%20package/main
   :target: https://github.com/LeapBeyond/scrubadub_address/actions?query=workflow%3A%22Python+package%22+branch%3Amain
   :alt:  Build Status
.. image:: https://img.shields.io/pypi/v/scrubadub_address.svg
   :target: https://pypi.org/project/scrubadub_address/
   :alt:  Version
.. image:: https://img.shields.io/pypi/dm/scrubadub_address.svg
   :target: https://pypi.org/project/scrubadub_address/
   :alt:  Downloads
.. image:: https://coveralls.io/repos/github/LeapBeyond/scrubadub_address/badge.svg?branch=master
   :target: https://coveralls.io/r/LeapBeyond/scrubadub_address
   :alt:  Test Coverage
.. image:: https://readthedocs.org/projects/scrubadub/badge/?version=latest
   :target: https://readthedocs.org/projects/scrubadub/?badge=latest
   :alt:  Documentation Status


Installation
------------

First libpostal needs to be installed.
Full instructions can be found in the `libpostal documentation <https://github.com/openvenues/libpostal#installation-maclinux>`_, but a summary is given below for linux installation:

.. code-block:: console

    $ sudo apt-get install curl autoconf automake libtool pkg-config
    $ git clone https://github.com/openvenues/libpostal
    $ cd libpostal
    $ ./bootstrap.sh
    $ ./configure --prefix=/usr/local/
    $ make -j4
    $ sudo make install

Once you have installed libpostal, the remaining python dependencies can be installed:

.. code-block:: console

    $ pip install pypostal scrubadub_address

New maintainers
---------------

`LeapBeyond <http://leapbeyond.ai/>`_ are excited to be supporting scrubadub with ongoing maintenance and development.
Thanks to all of the contributors who made this package a success, but especially `@deanmalmgren <https://github.com/deanmalmgren>`_, `IDEO <https://www.ideo.com/>`_ and `Datascope <https://datascopeanalytics.com/>`_.
