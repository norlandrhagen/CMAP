



.. _Jupyter: https://github.com/mdashkezari/opedia/blob/master/notebooks/SimpleExamples.ipynb


Eddy Sampling
=============




Code Tutorial
^^^^^^^^^^^^^


**Create a regional map using satellite and modeled data**

Notes:

The Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Satellite SST data set is a daily-global product with spatial resolution  1/4° X 1/4° .


Jupyter_


.. code-block:: python



    from opedia import eddy as EDD

    eddyTable = 'tblChelton'                                              # eddy table name
    startDate = '2014-04-01'                                              # eddy cores within the delimited space-time (start date)
    endDate = '2014-05-01'                                                # eddy cores within the delimited space-time (end date)
    lat1 = 23                                                             # eddy cores within the delimited space-time (start lat)
    lat2 = 29                                                             # eddy cores within the delimited space-time (end lat)
    lon1 = -161                                                           # eddy cores within the delimited space-time (start lon)
    lon2 = -151                                                           # eddy cores within the delimited space-time (end lon)
    fname = 'eddy'                                                        # figure filename (and/or shape filename)
    tables = ['tblSST_AVHRR_OI_NRT', 'tblDarwin_Nutrient_Climatology']    # list of varaible table names
    variables = ['sst', 'DON_darwin_clim']                         # list of variable names
    spatialTolerance = 0.3                                                # colocalizer spatial tolerance (+/- degrees)
    exportDataFlag = False                                                # export the cruise trajectory and colocalized data on disk
    depth1 = 0                                                            # depth range start (m)
    depth2 = 5                                                            # depth range end (m)


    cores = EDD.getEddies(eddyTable, startDate, endDate, lat1, lat2, lon1, lon2)
    EDD.colocalize(tables, variables, cores, spatialTolerance, depth1, depth2, exportDataFlag, fname, marker='-')



.. raw:: html

    <iframe src="../_static/tutorial_plots/eddy.html"  frameborder = 0  height="1000px" width="100%">></iframe>

|
|

GUI Tutorials
^^^^^^^^^^^^^
|

Mac OSX
^^^^^^^


.. raw:: html

    <iframe src="https://www.youtube.com/embed/uUDXwTyOfsk"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>


|
|

Windows
^^^^^^^

.. raw:: html

    <iframe src="https://www.youtube.com/embed/XhWMyocZYeI"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
