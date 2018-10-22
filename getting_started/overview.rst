


.. _Simmons: https://www.thesimmonsfoundation.org/


Overview
========

The **Simons Ocean Atlas** is an open source database service to unify, visualize, and analyze ocean data sets such as field campaign observations, remote sensing satellite data, and model outputs. The project is supported by the Simmons_ Foundation .


Project Mission
^^^^^^^^^^^^^^^



We, the oceanographers, have the best known job; it involves going to beach (and sea sometimes) and observe!

We probe the oceans to shed light on their underlying physical, chemical, and biological dynamics. Analyzing these observations, however, often require gathering more concurrent data such as satellite measurements and model estimates. Handling satellite and model data sets are particularly challenging because they:
are scattered all over the web and might not be trivial to discover
are massive in size
have different dimensions and resolutions.

The project's goal is to establish a unifying data structure and streamline the process of extracting data subsets, data visualization, and data integration. We propose that the space and time information should act as the linking chain between data sets and every single data point must be annotated with its own space and time data. Therefore, all data sets hosted in the Simons Ocean Atlas have the following simple data structure:

**Data structure**

+------+----------+-----------+------------------+------------------+
| Time | Latitude | Longitude | Depth (optional) | DATA VARIABLE(S) |
+------+----------+-----------+------------------+------------------+

The temporal and spatial resolution between data sets varies, but summaries of these coverages are provided within :ref:`Catalog`.


Project Process Flow
^^^^^^^^^^^^^^^^^^^^

Simons Foundation supports various ocean research programs and cruise expeditions. The results of these endeavors are shared with the scientific community and general public through the Simons Ocean Atlas. All data sets are first registered in formal digital archive repositories (such as zenodo.org) and obtain academically citable Digital Object Identifiers (DOI). The atlas also encompass a wide range of external data sets such as global satellite data and model outputs (see catalog [link to catalog]). We then ingest all data sets into a database system using the data structure mentioned above.  Finally, the application layer provides the user with the access to the database system where data set subsets can be retrieved and visualized.





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
