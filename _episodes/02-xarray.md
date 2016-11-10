---
title: "Using NetCDF in Python"
teaching: 20
exercises: 10
questions:
- "How can I look at datasets using Python?"
- "What operations are available?"
objectives:
- "Use the Xarray library to read a file"
- "Explain dimensions, variables and attributes"
- "Perform simple numpy operations on datasets"
keypoints:
- "Xarray lets you read NetCDF files in Python and inspect their contents"
- "NetCDF fields are made up of data + dimensions + metadata"
- "Numpy and Scipy let you perform calculations on fields"
---

There are quite a few libraries for working with climate data files in Python, here are a few:

 * [http://unidata.github.io/netcdf4-python/](http://unidata.github.io/netcdf4-python/)
 * [http://xarray.pydata.org](http://xarray.pydata.org)
 * [http://uvcdat.llnl.gov](http://uvcdat.llnl.gov)
 * [http://scitools.org.uk/iris](http://scitools.org.uk/iris)
 * [https://www.scipy.org/](https://www.scipy.org/)

Most are equally happy to open a file either on disk or over OPENDAP

We'll mostly look at `xarray` here, a 'higher-level' library for working with gridded data

> ## Example: Inspecting a file with xarray
> * Use xarray to open a file or OPENDAP link
> * What information can we see about the data?
>
> [Notebook](https://github.com/ScottWales/swc-climatedata/blob/gh-pages/data/02-xarray-basics.ipynb)
{: .callout}

Behind the scenes Xarray stores data using an optimised library called `numpy`,
with Xarray adding coordinates and metadata.

A lot of the time you don't want to work with the whole dataset, you need to
reduce it somehow. Perhaps you're only interested in a specific region, or want
to work with seasonal instead of monthly data

> ## Example: Slicing and dicing datasets
> * What are xarray's data subset options?
>
> [Notebook](https://github.com/ScottWales/swc-climatedata/blob/gh-pages/data/02-xarray-slicing.ipynb)
{: .callout}

> ## According to model data, what temperature was it in Melbourne today?
> The OPENDAP link to ACCESS1.3 RCP45 surface temperature is
> ~~~
> http://dapds00.nci.org.au/thredds/dodsC/ua6/authoritative/CMIP5/CSIRO-BOM/ACCESS1-3/rcp45/day/atmos/day/r1i1p1/latest/tas/tas_day_ACCESS1-3_rcp45_r1i1p1_20060101-20301231.nc
> ~~~
> {: .source}
{: .challenge}

> ## Example: Calculating the NINO 3.4 index
> The NINO 3.4 index is defined as the anomaly over the region (5N - 5S, 170W -
> 120W) compared to the historical average between 1961 and 1990
>
> [Notebook](https://github.com/ScottWales/swc-climatedata/blob/gh-pages/data/02-nino34.ipynb)
{: .callout}

> ## How do the RCP45 and RCP85 scenarios's NINO 3.5 index compare?
> OPENDAP links
>
> ~~~
> http://dapds00.nci.org.au/thredds/dodsC/ua6/authoritative/CMIP5/CSIRO-BOM/ACCESS1-3/historical/mon/atmos/Amon/r1i1p1/latest/ts/ts_Amon_ACCESS1-3_historical_r1i1p1_185001-200512.nc
> http://dapds00.nci.org.au/thredds/dodsC/ua6/authoritative/CMIP5/CSIRO-BOM/ACCESS1-3/rcp45/mon/atmos/Amon/r1i1p1/latest/ts/ts_Amon_ACCESS1-3_rcp45_r1i1p1_200601-210012.nc
> http://dapds00.nci.org.au/thredds/dodsC/ua6/authoritative/CMIP5/CSIRO-BOM/ACCESS1-3/rcp85/mon/atmos/Amon/r1i1p1/latest/ts/ts_Amon_ACCESS1-3_rcp85_r1i1p1_200601-210012.nc
> ~~~
> {: .source}
{: .challenge}

