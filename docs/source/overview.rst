========
Overview
========

WIVERNex-UK Chilbolton Campaign Dataset
---------------------------------------

This documentation describes the ground-based radar dataset collected 
at Chilbolton Obervatory in the UK for the WIVERNex-UK (WIVERN Phase-0 Campaigns Experiment in the UK),
funded by the European Space Agency (ESA) under
Contract no. 4000139702/22/NL/FF.

Level 1 calibrated data in NetCDF-4 format (see :ref:`file-format`) are provided
from the following radar: 

* 94GHz Galileo radar (ncas-radar-w-band-1)

The data are arranged into a series of 20 cases, 14 of which correcsp .  The data may be
read by a variety of standard packages including MATLAB, IDL and R, as well as by
tailored programs written in Python, C or Fortran.  For full
documentation of the NetCDF standard see https://www.unidata.ucar.edu/software/netcdf/.
Documentation is provided for the
:ref:`Python routines<raw-data-conversion>`
used in the processing chain leading to these Level 1 data.

A set of height-time quicklooks is also provided to enable the user to identify
periods of particular interest. An example is given below.

.. figure:: _static/example_quicklook_w-band.png
	   :width: 700 px
	   :align: center


:ref:`Python routines<quicklook-generation>` are provided for the production
of such quicklooks.  Specifically, they use the time-series data to generate
plots of radar equivalent reflectivity and of pulse-pair estimates of the
Doppler velocity.  No velocity unfolding is performed.


See also:

- wivern2-chilbolton source: https://github.com/longlostjames/wivern2_chilbolton
