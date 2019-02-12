.. _installation:

Installation
************

Installing via `conda`
======================

The simplest way to install ``kinomodel`` is via the `conda <https://conda.io>`_  package
manager.
Packages are provided on the `omnia Anaconda Cloud channel <http://anaconda.org/omnia>`_ for Linux, OS X, and Win platforms.
The `kinomodel Anaconda Cloud page <https://anaconda.org/kinomodel/yank>`_ has useful instructions and `download statistics <https://anaconda.org/omnia/kinomodel/files>`_.

If you are using the `anaconda <https://www.continuum.io/downloads/>`_ scientific Python distribution, you already have the ``conda`` package manager installed.
If not, the quickest way to get started is to install the `miniconda <http://conda.pydata.org/miniconda.html>`_ distribution, a lightweight minimal installation of Anaconda Python.

On ``linux``, you can install the Python 3.7 version into ``$HOME/miniconda3`` with:

.. code-block:: bash

   $ wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
   $ bash ./Miniconda3-latest-Linux-x86_64.sh -b -p $HOME/miniconda3
   $ export PATH="$HOME/miniconda3/bin:$PATH"

On ``osx``, you want to use the ``osx`` binary

.. code-block:: bash

   $ wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
   $ bash ./Miniconda3-latest-Linux-x86_64.sh -b -p $HOME/miniconda3
   $ export PATH="$HOME/miniconda3/bin:$PATH"

You may want to add the new ```$PATH`` extension to your ``~/.bashrc`` file to ensure Anaconda Python is used by
default.
Note that YANK will be installed into this local Python installation, so that you will not need to worry about
disrupting existing Python installations.

.. note::

   ``conda`` installation is the preferred method since all dependencies are automatically fetched and installed
   for you.

|

Release build
-------------

You can install the latest stable release build of ``kinomodel`` via the ``conda`` package with

.. code-block:: none

   $ conda config --add channels omnia --add channels conda-forge
   $ conda install kinomodel

This version is recommended for all users not actively developing new algorithms for alchemical free energy calculations.

.. note:: ``conda`` will automatically dependencies from binary packages automatically, including difficult-to-install packages such as OpenMM, numpy, and scipy. This is really the easiest way to get started.

|

Development build
-----------------

The bleeding-edge, absolute latest, very likely unstable development build of ``kinomodel` is available on `GitHub <http://github.com/inspiremd/kinomodel>`_.

.. warning:: Development builds may be unstable and are generally subjected to less testing than releases.  Use at your own risk!


Upgrading your installation
---------------------------

To update an earlier ``conda`` installation of YANK to the latest release version, you can use ``conda update``:

.. code-block:: bash

   $ conda update kinomodel

|
