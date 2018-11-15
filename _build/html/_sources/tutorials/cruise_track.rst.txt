
Visualize Cruise Track
======================



Visualize Data

Create depth profile plots using model and BGC-Argo float profiles.



Note:
Pisces model is a weekly-averaged global model with spatial resolution  1/2° X 1/2°  (data is available only at one-week intervals).

Darwin_Climatology is a monthly climatology version of the Darwin model with spatial resolution  1/2° X 1/2° .

Argo float data set has irregular temporal and spatial resolution.

.. code-block:: python


    from opedia import plotCruise as CRS

    DB_Cruise = True                 # < True > if cruise trajectory already exists in DB. < False > if arbiturary cruise file (e.g. virtual)
    source = 'tblSeaFlow'            # cruise table name or path to csv trajectory file
    cruise = 'SCOPE_16'              # cruise name, or file name of the csv trajectory file
    resampTau = '6H'                 # resample the cruise trajectory making trajectory time-space resolution coarser: e.g. '6H' (6 hourly), '3T' (3 minutes), ... '0' (ignore)
    fname = 'alongTrack'             # figure filename
    tables = ['tblSeaFlow', 'tblDarwin_Plankton_Climatology', 'tblCHL_OI_REP']    # list of varaible table names
    variables = ['picoeuk', 'picoeukaryote_c03_darwin_clim', 'chl']               # list of variable names
    spatialTolerance = 0.3           # colocalizer spatial tolerance (+/- degrees)
    exportDataFlag = False           # export the cruise trajectory and colocalized data on disk
    depth1 = 0                      # depth range start (m)
    depth2 = 5                       # depth range end (m)


    df = CRS.getCruiseTrack(DB_Cruise, source, cruise)
    df = CRS.resample(df, resampTau)
    loadedTrack = CRS.plotAlongTrack(tables, variables, cruise, resampTau, df, spatialTolerance, depth1, depth2, fname, exportDataFlag, marker='-', msize=30, clr='darkturquoise')


|
|

.. raw:: html

    <iframe src="../_static/tutorial_plots/alongTrack.html"  frameborder = 0  height="1000px" width="100%">></iframe>







GUI Tutorial
^^^^^^^^^^^^
|

Mac OSX
-------


.. raw:: html

    <iframe src="https://www.youtube.com/embed/cLY5R49JwCc"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>


|
|

Windows
-------

.. raw:: html

    <iframe src="https://www.youtube.com/embed/lHB21UWl-jw"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>

.. raw:: html

    <iframe src="https://www.youtube.com/embed/cn--aL9VElU"  frameborder = 0  height="700x" width="80%" allowfullscreen></iframe>
