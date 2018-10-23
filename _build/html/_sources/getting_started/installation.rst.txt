



Installation
============

**1. Install Anaconda Distribution**

https://www.anaconda.com/download/

**2. Set up database drivers (only required on macOS)**

.. code::

    $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ brew install unixodbc
    $ brew install freetds --with-unixodbc

**Install Additional Python Modules**


.. code::

    $ conda install shapely
    $ conda install fiona
    $ conda install -c conda-forge geopandas

    $ pip install opedia
