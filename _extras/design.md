---
layout: page
title: Design
permalink: /design/
---

## Concept

### Audience 
Early career researchers new to working with large climate datasets, with
some experience with Python programming

### Goals
 * Able to access and analyse large datasets such as CMIP5 efficiently
 * Able to set correct metadata on output files for publication

### Length
Half day

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
