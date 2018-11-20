


.. _Simons: https://www.simonsfoundation.org/




Overview
========



We, the oceanographers, have the best known job; it involves going to beach (and sea sometimes) and observe!

We probe the oceans to shed light on their underlying physical, chemical, and biological dynamics. Analyzing these observations, however, often require synthesizing more concurrent data such as satellite measurements and model estimates. Handling satellite and model data sets are particularly challenging because they:

* Are scattered all over the web and might not be trivial to discover

* Are massive in size

* Have different dimensions and resolutions.



The project's goal is to establish a unifying data structure and streamline the process of extracting data subsets, data visualization, and synthesis analysis. We propose that the space and time information should act as the linking chain between data sets and every single data point must be annotated with its own space and time data. Therefore, all data sets hosted in the Simons Ocean Atlas have the following simple data structure:


+------+-----+-----+-------------------+-----------------+-----+-----------------+
| time | lat | lon | depth {if exists} | <:math:`var_1`> | ... | <:math:`var_n`> |
+------+-----+-----+-------------------+-----------------+-----+-----------------+



Project Process Flow
^^^^^^^^^^^^^^^^^^^^

Simons Foundation supports various ocean research programs and cruise expeditions. The results of these endeavors are shared with the scientific community and general public through the Simons Ocean Atlas. All data sets are first registered in formal digital archive repositories (such as zenodo.org) and obtain academically citable Digital Object Identifiers (DOI). The atlas also encompass a wide range of external data sets such as global satellite data and model outputs (see  :ref:`Catalog`). We then ingest all data sets into a database system using the data structure mentioned above.  Finally, the API and application layers provide the user with the access to the database system where data set subsets can be retrieved and visualized.

.. figure:: ../_static/process_flow.png
   :scale: 60 %
   :align: center
