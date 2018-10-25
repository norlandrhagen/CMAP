
.. _Anaconda: https://www.anaconda.com/download/


Getting Started
===============


Installation
^^^^^^^^^^^^

The Simons Ocean Atlas is currently in development, but can be used in its present state.

The two options for using the Ocean Atlas to visualize data are either through a GUI (Graphical User Interface) for Windows and Mac OSX or through a command line interface for Windows, Mac OSX or Linux.

Future developments of the Simmons Ocean Atlas should be HTML browser based and operating system agnostic.

Windows
^^^^^^^

**1. Install Anaconda Distribution**

Anaconda_


**Install Additional Python Modules**


.. code-block:: rst

    $ conda install shapely
    $ conda install fiona
    $ conda install -c conda-forge geopandas

    $ pip install opedia



Mac OS X
^^^^^^^^


**1. Install Anaconda Distribution**

Anaconda_


**2. Install Additional Python Modules**

.. code-block:: rst

    $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ brew install unixodbc
    $ brew install freetds --with-unixodbc

    $ conda install shapely
    $ conda install fiona
    $ conda install -c conda-forge geopandas
    $ pip install opedia




Linux
^^^^^



**1. Install Anaconda Distribution**

Anaconda_

**Install Additional Python Modules**


.. code-block:: rst

    $ conda install -c anaconda unixodbc
    $ conda install -c anaconda freetds
    $ conda install shapely
    $ conda install fiona
    $ conda install -c conda-forge geopandas
    $ pip install opedia
