



.. _Jupyter: https://github.com/mdashkezari/opedia/blob/master/notebooks/SimpleExamples.ipynb


Plot Regional Map
=================




Code Tutorial
^^^^^^^^^^^^^


**Create a regional map using satellite and modeled data**

Notes:

The Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Satellite SST data set is a daily-global product with spatial resolution  1/4° X 1/4° .


Jupyter_


.. code-block:: python



    from opedia import plotRegional as REG


    tables = ['tblsst_AVHRR_OI_NRT', 'tblPisces_NRT']    # see catalog.csv  for the complete list of tables and variable names
    variables = ['sst', 'Fe']                            # see catalog.csv  for the complete list of tables and variable names
    startDate = '2016-04-30'
    endDate = '2016-04-30'
    lat1 = '10'
    lat2 = '70'
    lon1 = '-180'
    lon2 = '-80'
    depth1 = '0'
    depth2 = '0.5'
    fname = 'regional'
    exportDataFlag = False       # True if you you want to download data

    REG.regionalMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)




.. raw:: html

    <iframe src="../_static/RM_large.html"  frameborder = 0  height="1600px" width="100%">></iframe>


GUI Tutorial
^^^^^^^^^^^^
|

Mac OSX
-------


.. raw:: html

    <iframe src="https://www.youtube.com/embed/8zTh8nJ7pv0"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>


|
|

Windows
-------

.. raw:: html

    <iframe src="https://www.youtube.com/embed/XhWMyocZYeI"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
