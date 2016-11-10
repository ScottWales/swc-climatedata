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

Right tool for modifying attributes (add, delete change)

move variables, basic math

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


#### References
 * [http://nco.sourceforge.net/nco.html](http://nco.sourceforge.net/nco.html)
 * [https://code.zmaw.de/projects/cdo](https://code.zmaw.de/projects/cdo)


## NetCDF viewers

Panoply

Allows a variety of plot types, combine u and v vector data. Available at NCI on VDI only

Ncview, available at nci

Quick & simple viewer

#### References
 * [http://www.giss.nasa.gov/tools/panoply/](http://www.giss.nasa.gov/tools/panoply/)
 * [http://meteora.ucsd.edu/~pierce/ncview_home_page.html](http://meteora.ucsd.edu/~pierce/ncview_home_page.html)

> ## Example: Calculating a seasonal average from the command line
> Let's see how we can use nco and cdo
>
> [Notebook](https://github.com/ScottWales/swc-climatedata/blob/gh-pages/data/05-commandline.ipynb)
{: .callout}

> ## What tools do you use?
> There's a vast variety of tools out there, more than can be covered by me.
> Ask your neighbour what tools or libraries they use for data analysis
{: .discussion}
