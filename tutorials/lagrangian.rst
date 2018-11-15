



.. _Jupyter: https://github.com/mdashkezari/opedia/blob/master/notebooks/SimpleExamples.ipynb


Lagrangian Sampling
===================




Code Tutorial
^^^^^^^^^^^^^


**Create a regional map using satellite and modeled data**

Notes:

The Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Satellite SST data set is a daily-global product with spatial resolution  1/4° X 1/4° .


Jupyter_


.. code-block:: python



    from opedia import Lagrangian as LAG
    import pandas as pd

    fmt='%Y-%m-%d'
    dt = 24*3600                                                          # propagation time step (day seconds)
    direction = 1                                                         # propagation direction (forward/backward in time  <1> / <-1>)
    startDate = '2016-01-01'                                              # propagation start date
    endDate = '2016-02-01'                                                # propagation end date
    lat0 = 36                                                             # starting poin latitude
    lon0 = -73                                                            # starting poin longitude
    fname = 'Tracer'                                                      # figure filename (and/or shape filename)
    tables = ['tblSST_AVHRR_OI_NRT', 'tblDarwin_Plankton_Climatology']    # list of varaible table names
    variables = ['sst', 'diazotroph_c10_darwin_clim']                     # list of variable names
    spatialTolerance = 0.3                                                # colocalizer spatial tolerance (+/- degrees)
    exportDataFlag = False                                                # export the cruise trajectory and colocalized data on disk
    depth1 = 0                                                            # depth range start (m)
    depth2 = 5                                                            # depth range end (m)


    df = pd.DataFrame()
    df['time'], df['lat'], df['lon'] = LAG.propagate(direction, startDate, endDate, lat0, lon0, fmt, dt)
    LAG.plotAlongTrack(dt, fmt, tables, variables, df, spatialTolerance, depth1, depth2, exportDataFlag, fname, marker='-', msize=30, clr='darkturquoise')





.. raw:: html

    <iframe src="../_static/tutorial_plots/Tracer.html"  frameborder = 0  height="1600px" width="100%">></iframe>

|
|

GUI Tutorials
^^^^^^^^^^^^^
|

Mac OSX
^^^^^^^


.. raw:: html

    <iframe src="https://www.youtube.com/embed/yTwkmEcqsXE"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>


|
|

Windows
^^^^^^^

.. raw:: html

    <iframe src="https://www.youtube.com/embed/1splLq2z10M"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
