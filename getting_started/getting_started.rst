
.. _Anaconda Windows: https://www.anaconda.com/download/#windows
.. _Anaconda macOS: https://www.anaconda.com/download/#macos
.. _Anaconda Linux: https://www.anaconda.com/download/#linux



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

`Anaconda Windows`_

.. note::

    When installing Anaconda for windows make sure to choose the: "**Add Anaconda to my PATH environment variable**" option.

|

**Install Additional Python Modules**



.. note::

    Run Command Prompt as Administrator and then enter:

.. code-block:: none

    pip install opedia


|

macOS
^^^^^^^^


**Install Anaconda Distribution (Prefer Python 3+)**

`Anaconda macOS`_


**Install Additional Python Modules**

Open Terminal and then enter:

.. code-block:: none

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew install unixodbc
    brew install freetds --with-unixodbc

    pip install opedia



|

Linux
^^^^^



**Install Anaconda Distribution (Prefer Python 3+)**

`Anaconda Linux`_

**Install Additional Python Modules**

Open Terminal and then enter:

.. code-block:: none

    conda install -c anaconda unixodbc
    conda install -c anaconda freetds

    pip install opedia
