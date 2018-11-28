
.. _Install Anaconda Distribution (Prefer Python 3+): https://www.anaconda.com/download/#macos


macOS
=====


+----------------------------------------------------+
|`Install Anaconda Distribution (Prefer Python 3+)`_ |
+----------------------------------------------------+




**Install Additional Python Modules**

Open Terminal and then enter:

.. code-block:: none

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew install unixodbc
    brew install freetds --with-unixodbc

    pip install opedia
