:orphan:

.. _LCS:



LCS
***

.. |globe| image:: /_static/catalog_thumbnails/globe.png
   :scale: 10%
   :align: middle
.. |sat| image:: /_static/catalog_thumbnails/satellite.png
   :scale: 10%
   :align: middle



+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+
| Datset Name            |Spatial Coverage| Sensor Type |  Make       |     Spatial Resolution     | Temporal Resolution  |  Start Date  |  End Date  |
+========================+================+=============+=============+============================+======================+==============+============+
| :ref:`LCS`             |     |globe|    | |sat|       | Observation |     1/25° X 1/25°          |         Daily        |  2014-01-01  | 2017-05-01 |
+------------------------+----------------+-------------+-------------+----------------------------+----------------------+--------------+------------+

Dataset Description
*******************


.. figure:: /catalog/figures/LCS/Grid.png
   :width: 100%


**LCS (Lagrangian Coherent Structures)** is a daily-global altimetry-derived [link to altimetry data set] and gridded product calculating Finite-Time Lyapunov Exponents (FTLE). It characterizes the transport properties of the ocean surface currents from a Lagrangian frame of reference.

A grid of passive tracers (hypothetical massless particles) is initialized over the global domain with an initial uniform spacing of 4 km x 4 km. A flow map is then approximated by integrating particle trajectories for a fix period of time, :math:`\tau=15` days. At its fundamental levels, local Lyapunov exponents provide a metric for exponential rate of divergence for a pair of adjacent tracers:

.. math::
   \begin{equation} \label{Eq:Lyapunov}
   \Lambda = \lim_{|\delta x(t_0)| \to 0}  \lim_{t \to \infty} \frac{1}{t} \log \frac{\delta x(t)}{\delta x(t_0)}
   \end{equation}


such that :math:`\Lambda` is the Lyapunov exponent, and :math:`\delta x(t)`, :math:`\delta x(0)` represent the separation between the tracers at times :math:`t` and :math:`t_0`, receptively.


After integrating the particles for the fixed period of time, :math:`\tau=15`, FTLE fields are computed to demonstrate the local dispersion as well as local displacements (see example figures below). The particles can be integrated either forward or backward in time. The local maxima of the FTLE scalar field (ridges) can be interpreted as stable and unstable manifolds of the flow field in the case of forward and backward integration, respectively.


.. figure:: /catalog/figures/LCS/displacement_dispersion.png
   :width: 100%

Please refer to the documentation below for more detailed information regarding FTLE mathematical framework.


Table of Variables
******************

HTML table generated through python/sql script will live here

  
Data Source
***********

Opedia
Simons Ocean Atlas

https://github.com/mdashkezari/opedia/tree/master/CS
https://github.com/mdashkezari/opedia/tree/master/CS/docs

How to Acknowledge
******************


Version History
***************
