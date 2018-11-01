
Plot Regional Map
=================

Code Tutorial
^^^^^^^^^^^^^


**Create a regional map using satellite and modeled data**

Notes:

The Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Satellite SST data set is a daily-global product with spatial resolution  1/4° X 1/4° .

.. code:: python


    from opedia import plotRegional as REG


    tables = ['tblsst_AVHRR_OI_NRT', 'tblPisces_NRT']    # see catalog.csv  for the complete list of tables and variable names
    variables = ['sst', 'Fe']                            # see catalog.csv  for the complete list of tables and variable names
    startDate = '2016-04-30'
    endDate = '2016-04-30'
    lat1 = '20'
    lat2 = '50'
    lon1 = '-180'
    lon2 = '-100'
    depth1 = '0'
    depth2 = '0.5'
    fname = 'regional'
    exportDataFlag = False       # True if you you want to download data

    REG.regionalMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)



.. raw:: html

    <iframe src="../_static/RM_large.html"  frameborder = 0  height="1600px" width="100%">></iframe>


GUI Tutorial
^^^^^^^^^^^^


.. raw:: html

    <iframe src="https://www.youtube.com/embed/N8ZKF64xp1c?rel=0"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
