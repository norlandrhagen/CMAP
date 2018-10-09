
Catalog
=======
All data included in the Simmons Ocean Atlas must have Date, Time, Latitude and Longitude.

Temporal Data Extent
====================

.. image:: /_static/data_timeline_test.png
   :width: 700px
   :align: center

Spatial Data Extent
===================
.. code:: python

    # Get active layer:
    In [1]: layer = iface.activeLayer()

    # Print its name, and its number of features:
    In [2]: print(layer.name())
    Out[2]: 'DAMSELFISH Distributions'

    In [3]: print(layer.featureCount())
    Out[3]: 231

Data Variable Descriptions and Metadata
========================================
.. code-block:: console

    mkdir test
