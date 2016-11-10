---
title: "A trip to the library"
teaching: 20
exercises: 10
questions:
- "What data is available to me?"
objectives:
- "Learn about data catalogue and THREDDS services"
- "Explain netCDF file format and meta-data"
- "Use Syphon to get a list of data URLs"
keypoints:
- "NCI's public data catalogue is at https://datacatalogue.nci.org.au"
- "Additional datasets are available from ARCCSS CMS http://climate-cms.unsw.wikispaces.net/Data"
- "THREDDS allows you to selectively inspect and download data"
- "NetCDF format combines data and meta-data such as units and history"
- "The Siphon library can scan THREDDS indexes like a directory using Python"
---

The first step to analysing data is to find the data that you need. Is it public or access restricted? Can it be found locally or does it need to be downloaded first?

NCI has a catalogue of its public datasets at https://datacatalogue.nci.org.au. This lists a summary of each dataset, licence information, contact details and links to machine-readable information

NCI makes data available both through local file access and THREDDS

THREDDS allows users to access data services over the internet
 * OPENDAP allows programming languages to access remote netCDF data like it was a local file
 * HTTPServer allows you to download the entire file
 * NetcdfSubset allows you to download part of a file
 * NCML, ISO contain machine-readable metadata
 * UDDC gives a qualty report of the metadata
 * WMS / Web Mapping Service allows tools to create a web map of the data
 * WCS / Web Coverage Service is used by GIS tools to create maps

> ## Example: NCI's Data Catalogue
> * Explore NCI's data catalogue site, and the infomation and services that it provides
> * Use NCSS to download part of a NetCDF file
{: .callout}

ARCCSS CMS also maintains mirrors of a number of datasets at NCI, information can be found at http://climate-cms.unsw.wikispaces.net/Data. 
We make data available to researchers in a central location to reduce disk usage
We can help with obtaining datasets hosted outside of Australia

> ## What data do you require?
> Is there data that you need for your research that's not listed on the NCI or ARCCSS indexes? You can contact us at climate_help@nci.org.au to request data
{: .discussion}

> ## Example: Gathering URLs with Siphon
> Lets look at how we can use THREDDS from Python
>
> [Notebook](https://github.com/ScottWales/swc-climatedata/blob/gh-pages/data/01-siphon.ipynb)
{: .callout}

#### References
 * http://siphon.readthedocs.io/en/latest/
