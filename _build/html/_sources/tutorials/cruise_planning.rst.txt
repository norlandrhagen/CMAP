
.. _Jupyter Notebook: https://github.com/mdashkezari/opedia/blob/master/notebooks/Gradients3.ipynb


Cruise Planning
===============


`Jupyter Notebook`_


Example 1: Surface Maps (Satellite)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Create surface maps using near-real-time satellite data.**

Notes:
- **Not all plots are displayed in this tutorial due to html size issues**
- Pisces model is a weekly-averaged global model with spatial resolution  1/2° × 1/2°  (data is available only at one-week intervals).
- Satellite SST data set is a daily-global product with spatial resolution   1/4° × 1/4° .


Code Tutorial
-------------

.. code-block:: python

    from opedia import plotRegional as REG

    tables = ['tblsst_AVHRR_OI_NRT', 'tblAltimetry_NRT', 'tblCHL_OI_NRT', 'tblLCS_NRT', 'tblLCS_NRT', 'tblWind_NRT', 'tblSSS_NRT']
    variables = ['sst', 'sla_nrt', 'chl_nrt', 'ftle_nrt', 'disp_nrt', 'wind_stress', 'sss']
    startDate = '2019-03-02'
    endDate = '2019-03-02'
    lat1, lat2 = 10, 70
    lon1, lon2 = -180, -80
    depth1, depth2 = 0, 0.5
    fname = 'surface_satellite'
    exportDataFlag = False       # True if you you want to save data in .csv format

    REG.regionalMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)

.. raw:: html

    <iframe src="../_static/tutorial_plots/surface_satellite.html"  frameborder = 0  height="1000px" width="100%">></iframe>



|




Example 2: Surface Organisms Maps (Model)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Create surface maps using Darwin monthly climatology data.**

Notes:

- Darwin_Climatology is a monthly climatology version of the Darwin model with spatial resolution  1/2° × 1/2°

Code Tutorial
-------------


.. code-block:: python

    from opedia import plotRegional as REG


    tables = ['tblDarwin_Plankton_Climatology', 'tblDarwin_Plankton_Climatology']
    variables = ['prokaryote_c01_darwin_clim', 'prokaryote_c02_darwin_clim']
    startDate = '2019-03-02'
    endDate = '2019-03-02'
    lat1, lat2 = 10, 70
    lon1, lon2 = -180, -80
    depth1, depth2 = 0, 5
    fname = 'organism_model'
    exportDataFlag = False       # True if you you want to save data in .csv format

    REG.regionalMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)

.. raw:: html

    <iframe src="../_static/tutorial_plots/organism_model.html"  frameborder = 0  height="1000px" width="100%">></iframe>


|




Example 3: Surface Maps (Model)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Create a surface maps using near-real-time model data.**

Notes:

- Pisces model is a weekly-averaged global model with spatial resolution 1/2° × 1/2° (data is available only at one-week intervals).

Code Tutorial
-------------


.. code-block:: python

    from opedia import plotRegional as REG


    tables = ['tblMercator_MLD_NRT', 'tblPisces_NRT', 'tblPisces_NRT', 'tblPisces_NRT', 'tblPisces_NRT']
    variables = ['mld_nrt', 'NO3', 'PO4', 'Fe', 'O2']
    startDate = '2019-03-02'
    endDate = '2019-03-02'
    lat1, lat2 = 10, 70
    lon1, lon2 = -180, -80
    depth1, depth2 = 0, 0.5
    fname = 'surface_model'
    exportDataFlag = False       # True if you you want to save data in .csv format

    REG.regionalMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)

.. raw:: html

    <iframe src="../_static/tutorial_plots/surface_model.html"  frameborder = 0  height="1000px" width="100%">></iframe>


|


Example 4: Section plots (Model)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Create section maps using monthly climatology data from Darwin and near-real-time data from PISCES model.**

Notes:

- Darwin_Climatology is a monthly climatology version of the Darwin model with spatial resolution  1/2° × 1/2°
- Pisces model is a weekly-averaged global model with spatial resolution 1/2° × 1/2° (data is available only at one-week intervals).

Code Tutorial
-------------

.. code-block:: python

    from opedia import plotSection as SEC

    tables = ['tblDarwin_Nutrient_Climatology', 'tblDarwin_Nutrient_Climatology', 'tblPisces_NRT', 'tblPisces_NRT', 'tblPisces_NRT', 'tblPisces_NRT']
    variables = ['NH4_darwin_clim', 'SiO2_darwin_clim', 'Fe', 'NO3', 'CHL', 'PO4', 'O2']
    startDate = '2019-03-02'
    endDate = '2019-03-02'
    lat1, lat2 = 20, 55
    lon1, lon2 = -159, -157
    depth1, depth2 = 0, 1000
    fname = 'SEC'
    exportDataFlag = False                  # True if you you want to save data in .csv format

    SEC.sectionMap(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)

.. raw:: html

    <iframe src="../_static/tutorial_plots/SEC.html"  frameborder = 0  height="1000px" width="100%">></iframe>
