---
title: "Using NetCDF in Python"
teaching: 30
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

 * Load a single file with Xarray & inspect contents
   * See variables, attributes. Compare with `ncdump`

 * Average & calculate anomaly over NINO34 area
   * Introduce numpy
   * Create a netcdf file
