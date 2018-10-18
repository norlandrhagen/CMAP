
Overview
========


**Project Mission**

The Simons Ocean Atlas is an open source database service to integrate, visualize, and analyze ocean datasets such as satellite data, in-situ observations, and model outputs.
The project is supported by Simons Foundation.


**Data structure**


All data in the Simmons Ocean Atlas should be structured in the format:

+------+------+----------+-----------+------------------+
| DATE | TIME | LATITUDE | LONGITUDE | DATA VARIABLE(S) |
+------+------+----------+-----------+------------------+

The temporal and spatial resolution between data sets varies, but summaries of these coverages are provided within :ref:`Catalog`.



Installation
^^^^^^^^^^^^

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
