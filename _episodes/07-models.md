---
title: "Analysing model output"
teaching: 30
exercises: 10
questions:
- "How can I analyse model output?"
objectives:
- "Use Iris to load a Unified Model file"
- "Explore auxillary dimensions"
- "Create a Cartopy plot"
keypoints:
- "There are lots of tools for working with climate data beyond what's been covered here"
---

As a final topic, let's look at another library for working with climate data, Iris.

Iris represents variables as 'data cubes', which like Xarray combine data, co-ordinates and metadata

Iris will also create 'auxillary co-ordinates', that are alternate views of the
other co-ordinates e.g. model and pressure levels

Iris will also load GRIB2 (used in weather forecasting) and Unified Model
files, the atmospheric model used in ACCESS

> ## Example: Inspecting a model output file with Iris
> Let's look at what we can see in an output file from the ACCESS model
{: .callout}

> ## What are the differences between Iris and Xarray's datasets?
> Try loading the same NetCDF file in each - do they show the same information?
{: .challenge}

Like Xarray iris has tools for indexing and reducing data. It can also convert GRIB2 or UM files to CF-NetCDF

> ## Example: Iris cube operations
> What can we do with an Iris cube?
{: .callout}

## Plotting your data

Just like netCDF libraries there are a number of ways you can go about plotting
data, inside and outside of Python.

http://matplotlib.org/
http://scitools.org.uk/cartopy/
http://geo.holoviews.org/

> ## Example: Plotting with Matplotlib and Cartopy
> Let's explore options for creating plots
{: .callout}

> ## Create an interactive plot in Ipython
> Check out the [GeoViews documentation](http://geo.holoviews.org/) and create
> a plot in Ipython showing how surface temperature in Australia changes over a
> year
>
> Start by finding a relevant dataset in THREDDS and loading it into Xarray
{: .challenge}

http://scitools.org.uk/iris/
http://scitools.org.uk/cartopy/

 * Load a model data cube with Iris
   * Different level types, aux dimensions

 * Plot the difference between model and ERA-Interim surface temp with Cartopy
   * Python plotting
