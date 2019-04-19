
.. _Github: https://github.com/mdashkezari/opedia/


API Reference
=============


.. note::
  API is currently in development


|


Github_


.. class:: /Catalog GET

    Access metadata on datasets available in the repository.

    Parameters: None

    Returns: chunk-encoded data where each chunk is an array of metadata objects describing data available from the API.

    The returned metadata objects have the following attributes:

    .. attribute:: variable(string)

     The short name of the variable

    .. attribute:: longName(string)

     The full name of the variable

    .. attribute:: 	unit(string)

     The unit of measurement of the data

    .. attribute:: 	make(string)

     Observation, Model or Assimilation

    .. attribute:: 	sensor(string)

     The type of sensor used to collect the data

    .. attribute:: processLevel(string)

     Near-Real-Time, Reprocessed or Forecast

    .. attribute:: temporalResolution(string)

     The frequency of collection

    .. attribute:: spatialResolution(string)

     The spatial domain of the data

    .. attribute:: comment(string)

     Additional comment about the variables

    .. attribute:: datasetName(string)

     The name of the dataset

    .. attribute:: 	dataSource(string)

     Name of lab, project or organization where data originated

    .. attribute:: distributor(string)

     Organization responsible for distributing the data

    .. attribute:: datasetDescription(string)

     The full description of the dataset

    .. attribute:: 	datasetID(int)

     Database linking ID

    .. attribute:: id(int)

     Unique ID for variable

    .. attribute:: 	tableName(string)

     The table storing this variable in the CMAP data repository

    .. attribute:: keywords(string)

     A list of space-separated keywords describing the variable
