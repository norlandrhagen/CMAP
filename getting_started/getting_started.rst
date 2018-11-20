
.. _Anaconda: https://www.anaconda.com/download/



Getting Started
===============




Installation
^^^^^^^^^^^^

The Simons Ocean Atlas is currently in development, but can be used in its present state.
The two options for using the Ocean Atlas are either through a GUI (Graphical User Interface) for Windows and macOS or through a command line interface for Windows, macOS or Linux.
Future developments of the Simons Ocean Atlas should be browser based and operating system agnostic.

Windows
^^^^^^^

**Install Anaconda Distribution (Prefer Python 3+)**

Anaconda_



**Install Additional Python Modules**



.. code-block:: none

    $ pip install opedia



macOS
^^^^^^^^


**Install Anaconda Distribution (Prefer Python 3+)**

Anaconda_


**Install Additional Python Modules**

.. code-block:: none

    $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ brew install unixodbc
    $ brew install freetds --with-unixodbc

    $ pip install opedia




Linux
^^^^^



**Install Anaconda Distribution (Prefer Python 3+)**

Anaconda_

**Install Additional Python Modules**


.. code-block:: none

    $ conda install -c anaconda unixodbc
    $ conda install -c anaconda freetds

    $ pip install opedia
