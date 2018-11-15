



.. _Jupyter: https://github.com/mdashkezari/opedia/blob/master/notebooks/SimpleExamples.ipynb


Section Plot
============



Code Tutorial
^^^^^^^^^^^^^


**Create a regional map using satellite and modeled data**

Notes:

The Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Satellite SST data set is a daily-global product with spatial resolution  1/4° X 1/4° .


Jupyter_


.. code-block:: python



    from opedia import plotSection as SEC

    tables = ['tblDarwin_Nutrient_Climatology']    # see catalog.csv  for the complete list of tables and variable names
    variabels = ['CDOM_darwin_clim']                            # see catalog.csv  for the complete list of tables and variable names



    dt1 = '2016-04-30'   # PISCES is a weekly model, and here we are using monthly climatology of Darwin model
    dt2 = '2016-04-30'
    lat1, lat2 = 23, 55
    lon1, lon2 = -159, -157
    depth1, depth2 = 0, 3597
    fname = 'sectional'
    exportDataFlag = False       # True if you you want to download data

    SEC.sectionMap(tables, variabels, dt1, dt2, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)


.. raw:: html

    <iframe src="../_static/tutorial_plots/sectional.html"  frameborder = 0  height="600px" width="100%">></iframe>


|
|


GUI Tutorials
^^^^^^^^^^^^^
|

Mac OSX
^^^^^^^


.. raw:: html

    <iframe src="https://www.youtube.com/embed/v1NLEgqgYjo"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>


|
|

Windows
^^^^^^^

.. raw:: html

    <iframe src="https://www.youtube.com/embed/iv13GZ9Uomo"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
