.. image:: https://travis-ci.org/Oslandia/py3dtiles.svg?branch=master
    :target: https://travis-ci.org/Oslandia/py3dtiles

.. image:: https://badge.fury.io/py/py3dtiles.svg
    :target: https://badge.fury.io/py/py3dtiles

=========
py3dtiles
=========

p3dtiles is a Python tool and library for manipulating `3D Tiles`_.

.. _3D Tiles: https://github.com/AnalyticalGraphicsInc/3d-tiles

**CLI Features**

* Convert pointcloud LAS and XYZ files to a 3D Tiles tileset (tileset.json + pnts files)
* Merge pointcloud 3D Tiles tilesets into one tileset
* Read pnts and b3dm files and print a summary of their contents

**API features**

* Read/write pointcloud (pnts) and batched 3d model format

py3dtiles is distributed under the Apache 2 Licence.


Installation
------------

From sources
~~~~~~~~~~~~

To use py3dtiles from sources:

.. code-block:: shell

    $ apt install git python3 python3-pip virtualenv libopenblas-base liblas-c3
    $ git clone https://github.com/Oslandia/py3dtiles
    $ cd py3dtiles
    $ virtualenv -p /usr/bin/python3 venv
    $ . venv/bin/activate
    (venv)$ pip install -e .
    (venv)$ python setup.py install

If you wan to run unit tests:

.. code-block:: shell

    (venv)$ pip install nose
    (venv)$ nosetests
    ...

With docker
~~~~~~~~~~~~

Build the py3dtiles docker image:

.. code-block:: shell

    $ git clone https://github.com/Oslandia/py3dtiles
    $ cd py3dtiles
    $ docker build -t py3dtiles .

Use the py3dtiles docker image :

.. code-block:: shell

    $ docker run -it --rm py3dtiles
    $ docker run -it --rm py3dtiles py3dtiles --help
    $ docker run -it --rm py3dtiles py3dtiles info... See Command line usage section



Licence
-------

py3dtiles is distributed under the Apache 2 Licence.

Links
-------

GitHub repository: https://github.com/Oslandia/py3dtiles

Documentation : https://oslandia.github.io/py3dtiles
