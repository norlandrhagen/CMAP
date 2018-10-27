
Plot Time Series
================




**Create a Time Series plot using satellite and modeled data**




**Note:**

Pisces model is a weekly-averaged global model with spatial resolution 1/2° X 1/2° (data is available only at one-week intervals).

Satellite wind data set is a 6-hourly global product with spatial resolution 1/4° X 1/4° .

Satellite Altimetry data set is a daily-global product with spatial resolution 1/4° X 1/4° .

.. code:: python


    from opedia import plotTS as TS

    tables = ['tblWind_NRT', 'tblAltimetry_REP', 'tblPISCES_NRT']
    variables = ['wind_stress', 'sla', 'NO3']
    startDate = '2016-03-29'
    endDate = '2016-04-29'
    lat1 = '25'
    lat2 = '30'
    lon1 = '-160'
    lon2 = '-155'
    depth1 = '0'
    depth2 = '5'
    fname = 'TS'
    exportDataFlag = False      # True if you you want to download data

    TS.plotTS(tables, variables, startDate, endDate, lat1, lat2, lon1, lon2, depth1, depth2, fname, exportDataFlag)







.. raw:: html

    <iframe src="../_static/TS.html"  frameborder = 0  height="1600px" width="100%">></iframe>
