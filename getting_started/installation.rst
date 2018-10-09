
System Requirements
===================
- Anaconda Distribution Python 2.7 or 3.7
- Python must be in the system path
- Additional Python modules

   - pyodbc
   - dropbox
   - geopandas


Installation
============

1. Install Anaconda Distribution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
https://www.anaconda.com/download/

2. Set up database drivers (only required on macOS)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. code-block:: console

    $ mkdir test
    $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ brew install unixodbc
    $ brew install freetds --with-unixodbc

3. Install Additional Python Modules
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: console

    $ conda update --all
    $ conda install pyodbc
    $ conda install dropbox
    $ conda install -c conda-forge geopandas
