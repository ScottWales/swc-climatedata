---
layout: page
title: Design
permalink: /design/
---

## Concept

describe who the lesson is for, what its overall goals are, and how long it is
going to be. For example, the lesson might be for people who have taught
themselves how to write page-long statistical analyses in R using RStudio, but
have never written functions or run programs from the Unix shell prompt. Its
overall goal might be to teach them how to write modular multi-page programs
and how to use dplyr to regularize their analyses, and the time allotted might
be half a day. It’s often helpful to use concept maps in this stage.

*Audience*: Early career researchers new to working with large climate datasets, with
some experience with Python programming

*Goals*:  
 * Able to access and analyse large datasets such as CMIP5 efficiently
 * Able to set correct metadata on output files for publication

*Length*: Half day

## Summative Assessment:
 * Calculate NINO34 index on official ACCESS 1.3 dataset, storing output as CF-netCDF  
    Covers concepts:
     * Catalogue
     * THREDDS
     * Syphon
     * Xarray
     * Dask
     * CF-Metadata

## Formative Assessment:

 * Search for datasets on the Catalogue
   * Explore available datasets, THREDDS functionality

 * Get URLs for a data run with Syphon
   * Collect list of files holding the ocean surface temperature

 * Load a single file with Xarray & inspect contents
   * See variables, attributes. Compare with `ncdump`

 * Average & calculate anomaly over NINO34 area
   * Introduce numpy

 * Subset the data, explore chunking options
   * Explain Dask, memory limits

 * Load multiple files with chunking
   * Compare loops vs whole-array operations

 * Use cdo/nco to calculate seasonal average
   * Importance of metadata, history attribute
   * Quick plots with ncview

 * Prepare publication, DOIs, ANDS, Orchid
   * http://climate-cms.unsw.wikispaces.net/Data+publishing+guidelines
   * Data citation, reproducible data

 * Load a model data cube with Iris
   * Different level types, aux dimensions

 * Plot the difference between model and ERA-Interim surface temp with Cartopy
   * Python plotting
