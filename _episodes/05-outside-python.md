---
title: "Outside Python"
teaching: 15
exercises: 5
questions:
- "How can I work with climate data outside of Python?"
objectives:
- ""
keypoints:
- ""
---

## Manipulating NetCDF files

ncdump
ncdiff

There are a whole bunch of pre-made analyses in the CDO and NCO libraries

Available at NCI through modules, or on Conda in the 'conda-forge' channel

Work with files on disk or over OPENDAP

Easier to use existing tools than writing your own

Come with OpenMP threading optimisations

NCO:

Concatenate files, ensemble averaging, 

Lots of options, complex 'kitchen-sink' operator

Rename variables, move variables, basic math

CDO:
Basic stats for each variable (min, mean, max)
cdo infon FILE
- Check for extremes

Compare two files
cdo diff FILEA FILEB
- Check model reproducibility

* Modificiation
  - Masks, attributes
* Arithmetic
* Statistics
* Correlations
* Interpolation

http://nco.sourceforge.net/nco.html
https://code.zmaw.de/projects/cdo

## NetCDF viewers

Panoply

Allows a variety of plot types, combine u and v vector data. Available at NCI on VDI only

http://www.giss.nasa.gov/tools/panoply/

Ncview, available at nci

Quick & simple viewer

http://meteora.ucsd.edu/~pierce/ncview_home_page.html


 * Use cdo/nco to calculate seasonal average
   * Importance of metadata, history attribute
   * Quick plots with ncview
