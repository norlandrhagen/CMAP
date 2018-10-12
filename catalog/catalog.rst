
.. _Catalog:


Data Haronization
^^^^^^^^^^^^^^^^^
All data in the Simmons Ocean Atlas should be structured in the format:

+------+------+----------+-----------+------------------+
| DATE | TIME | LATITUDE | LONGITUDE | DATA VARIABLE(S) |
+------+------+----------+-----------+------------------+

Data Sets Available
===================

.. |globe| image:: /_static/catalog_thumbnails/globe.png
   :scale: 10%
   :align: middle
.. |sat| image:: /_static/catalog_thumbnails/satellite.png
   :scale: 10%
   :align: middle
.. |float| image:: /_static/catalog_thumbnails/buoy.png
   :scale: 10%
   :align: middle
.. |cruise| image:: /_static/catalog_thumbnails/cruise.jpg
   :scale: 10%
   :align: middle

.. |comp| image:: /_static/catalog_thumbnails/comp.png
   :scale: 10%
   :align: middle

.. |seaflow| image:: /_static/catalog_thumbnails/seaflow.png
   :scale: 15%
   :align: middle

.. |argo| image:: /_static/catalog_thumbnails/argo.png
   :scale: 10%
   :align: middle

Spatial and Temporal Resolutions are approximate - for more detail see each dataset documentation

+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
| Datset Name            |Spatial Coverage| Sensor Type |  Make       |     Spatial Resolution     | Temporal Resolution  |  Start Date  |  End Date  |
+========================+================+=============+=============+============================+======================+==============+============+
| :ref:`Argo`            |     |float|    |  |argo|     | Observation |      ~ 3° X 3°             |        Irregular     |  2002-09-08  | 2018-06-07 |
+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
| :ref:`SST`             |     |globe|    | |sat|       | Observation |     1/4° X 1/4°            |         Daily        |  2013-01-01  | 2017-05-15 |
+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
| :ref:`SeaFlow`         |     |seaflow|  | |cruise|    | Observation |     1/2° X 1/2°            |    Three Minutes     |  2010-22-10  | 2017-06-13 |
+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
| :ref:`Darwin`          |     |globe|    | |comp|      |   Model     |     1/2° X 1/2°            |         Monthly      |  2013-08-11  | 2013-09-04 |
+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
