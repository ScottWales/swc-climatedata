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

If the right data is present (even if unstructured) data can be published in a
matter of days

#### Resources
 * [http://www.ands.org.au/working-with-data/metadata](http://www.ands.org.au/working-with-data/metadata)

> ## Example: CF-netCDF metadata
> To publish our NINO 3.4 data we'll first need to add some metadata
{: .callout}

### Data management plans

When you apply for a grant from the ARC you may need to provide a data
management plan, which provides information on where your data is stored and
how it's made available to other researchers

Institutions also require data management plans, especially for students -
thesis related data needs to be kept in an institutional archive for a number
of years after graduation


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

#### Resources
 * [http://www.ands.org.au/working-with-data/citation-and-identifiers](http://www.ands.org.au/working-with-data/citation-and-identifiers)
 * [https://guides.github.com/activities/citable-code/](https://guides.github.com/activities/citable-code/)
 * [https://www.nhmrc.gov.au/grants-funding/policy/nhmrc-and-arc-statement-open-researcher-and-contributor-id-orcid](https://www.nhmrc.gov.au/grants-funding/policy/nhmrc-and-arc-statement-open-researcher-and-contributor-id-orcid)
 * [https://zenodo.org/](https://zenodo.org/)

