---
title: "Publishing Data"
teaching: 15
exercises: 5
questions:
- "How can I make my own data available to others?"
- "How should I cite datasets?"
objectives:
- "Explain the publication process"
- "Explain DOIs, ORCID, Zenodo"
- "Data management plans"
keypoints:
- "Publishing datasets can be a requirement of grants or journals"
- "CMS is happy to assist with publication - climate_help@nci.org.au"
---

### Metadata

Metadata is important for others to be able to understand and use your data.
The standard in the climate area is [CF-NetCDF](http://cfconventions.org/),
which has standard variable and dimension names that make it possible to
compare results from different centres agains each other

Without metadata it is much harder to get tools like THREDDS to work, harder
for other researchers to use - what are the units for this field?

It's easier to collect information as you go, tools will generally preserve
attributes. Saves having to backtrack through everything at the end

Metadata is for both single files as well as groups of files

If the right data is present (even if unstructured) data can be published in a
matter of days

Attribute convention for data discovery is a good list of recommended attributes

History give a view on how the file was created, use timestamps

NCO's `ncatted` can edit attributes

~~~
ncatted --attribute NAME,VARIABLE,MODE,TYPE,VALUE input.nc output.nc
~~~
{: .source}

#### Resources
 * [http://www.ands.org.au/working-with-data/metadata](http://www.ands.org.au/working-with-data/metadata)
 * [http://cfconventions.org](http://cfconventions.org)
 * [http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery](http://wiki.esipfed.org/index.php/Attribute_Convention_for_Data_Discovery)

> ## Example: CF-netCDF metadata
> To publish our NINO 3.4 data we'll first need to add some metadata
{: .callout}

### Data management plans

When you apply for a grant from the ARC you may need to provide a data
management plan, which provides information on where your data is stored and
how it's made available to other researchers

Institutions also require data management plans, especially for students -
thesis related data needs to be kept in an institutional archive for a number
of years after graduation.

Think about licencing, creative commons is ANDS recommendation

#### Resources
 * [http://climate-cms.unsw.wikispaces.net/Data+publishing+guidelines](http://climate-cms.unsw.wikispaces.net/Data+publishing+guidelines)
 * [http://www.ands.org.au/working-with-data/data-management/data-management-plans](http://www.ands.org.au/working-with-data/data-management/data-management-plans)

> ## How do you manage your own data?
> Think about your own project
> * Will data need to be published when you publish papers or apply for grants?
> * Where is your data stored?
>   * Is it backed up?
>   * How long can it stay there?
> * Do you have documentation and metadata alongside your files?
> * Is your data licensed?
{: .challenge}

### Citing data

Papers, datsets and model code can be assigned a permanent identifier, called a
DOI (digital object identifier) so that others can cite it.

You can follow a DOI link to the canonical location using the website https://www.doi.org/

Papers are assigned DOIs by the publisher. NCI can arrange for DOIs for data
published and served on their systems, your institution may be able to help as
well

ANDS partners with ORCID, a researcher ID system, to match datasets with authors

ARC encourages researchers to sign up

Not-for-profit organisation linking researchers with publications and data

Code is also data, and important to preserve and cite! Keep your code in
version control (github, bitbucket, gitlab). You can assign a DOI to a specific
code version, either through ANDS or tools like CERN's Zenodo

> ## Recommended citation formats
> Creator (PublicationYear). Title. Publisher. Identifier
>
> Creator (PublicationYear). Title. Version. Publisher. ResourceType. Identifier
> 
> [https://www.datacite.org/cite-your-data.html](https://www.datacite.org/cite-your-data.html)
{: .callout}

#### Resources
 * [http://www.ands.org.au/working-with-data/citation-and-identifiers](http://www.ands.org.au/working-with-data/citation-and-identifiers)
 * [https://guides.github.com/activities/citable-code/](https://guides.github.com/activities/citable-code/)
 * [https://www.nhmrc.gov.au/grants-funding/policy/nhmrc-and-arc-statement-open-researcher-and-contributor-id-orcid](https://www.nhmrc.gov.au/grants-funding/policy/nhmrc-and-arc-statement-open-researcher-and-contributor-id-orcid)
 * [https://zenodo.org/](https://zenodo.org/)

## Getting help

ARCCSS CMS are happy to help publish your data. We have a dedicated data
manager who works with NCI and ANDS to make sure your data is available and
citable, email **climate_help@nci.org.au**
