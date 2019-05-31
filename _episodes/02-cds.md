---
title: "Copernicus Climate Data Store (CDS)"
teaching: 0
exercises: 0
questions:
- "Where to get Climate data?"
- "What is Copernicus CDS?"
- "How to retrieve Copernicus Climate data?"
- "What are netCDF and GRIB formats?"
- "What is CDS Toolbox?"
objectives:
- "Get an overview of various aspects of CDS Toolbox"
keypoints:
- "CDS Essential Information"
- "Retrieve data from the CDS web interace"
- "Visualize Climate data with the CDS Toolbox"
- "netCDF and GRIB data formats"
---

# Where to get Climate data?

There are many online services to get climate data, and it is often difficult to know which ones are up-to date and which resources to trust. Also different services provide different Application Programming Interfaces (API), use different terminologies, different file formats etc.,  which make it difficult for new users to master them all. Therefore in this lesson, we will be focusing on the [Copernicus Climate Change Service (C3S)](https://climate.copernicus.eu/).


# Copernicus Climate Change Service (C3S)

This is a service operated by the [European Centre for Medium-range Weather Forecasts (ECMWF)](https://www.ecmwf.int/) on behalf of the European Union. The [C3S](https://climate.copernicus.eu/) combines observations of the climate system with the latest science to develop **authoritative**, **quality-assured** information about the past, current and future states of the climate in Europe and worldwide.

<img src="../fig/C3S_frontpage.png" />

# The Climate Data Store (CDS)

This is a web portal providing a single point of access to a wide range of information. This includes observations (i.e., in-situ measurements, remote sensing data, etc.), historical climate data records, estimates of Essential Climate Variables (ECVs) derived from Earth observations, global and regional climate reanalyses of past observations, seasonal forecasts and climate projections.

> ## Climate Data Store (CDS) Registration
> To be able to use CDS services, you need to [register](https://cds.climate.copernicus.eu/user/login?destination=%2F%23!%2Fhome).
> Registration to the Climate Data Store (CDS) is free as well as access to
> climate data.
>
{: .callout}

Before starting, and once registred, login to the Climate Data Store (CDS).

<img src="../fig/CDS_login.png" width="80%"/>


## Search data in the Climate Data Store

Once login, click on the [Search](https://cds.climate.copernicus.eu/cdsapp#!/search) button:

<img src="../fig/CDS_search.png" width="80%"/>

If you click on "Product Type", you will get the list of available climate data types:

- Climate projections
- Reanalysis
- Satellite observations
- Seasonal forecasts
- Sectorial climate indices

> ## Which product type should I choose?
> You probably recognize the first 3 product types from the previous
> lesson, so let us do a small exercise.
>
> Alice is a Master's student working on draught in Europe over the period 1998-2018, and she wants to look at precipitation data for summer months in 2003 to start with (because she heard about a period of excessively hot and dry weather occuring then).
>
> Which product(s) types can she use?
>
> Which criteria could she use to make her final choice?
> > ## Solution
> > Alice could use:
> > - Climate projections
> > - Reanalysis
> > - Satellite observations
> >
> > and her final choice depends on the variable, the spatial and temporal resolution.
> {: .solution}
>
{: .challenge}

You can also search by entering a key word:
- reanalysis
- cmip
- temperature
- precipitation, etc.

When you search, you can make sure you only get datasets (and not documentation, etc.) by selecting the tab "Datasets"

<img src="../fig/CDS_tab_datasets.png" width="80%"/>

As you can see, it is important to know what you are looking for before starting to download datasets. We will see in the next section that the size of the datasets can also be an important criteria to take into account before starting downloading Climate data.

## Downloads data from the Climate Data Store

We are nearly there! And the best is to try it out.

Let's search for the last available re-analysis. We can search for "ERA5" and it will return the list of available datasets:

<img src="../fig/CDS_ERA5_search.png" width="80%"/>

> ## Single level versus pressure levels
>
> Let's stop here and discuss the results of our search:
> - single levels are usually for variables available at (or close) to the surface.
> - data on pressure levels give information on the vertical structure of the atmosphere.
>
> For many practical applications, using single level (surface) data is sufficient.
{: .callout}

We will select [ERA5 monthly averaged data on single levels from 1979 to present](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=overview).

<img src="../fig/CDS_ERA5_download.png" width="80%"/>

> ## License
> To be able to download datasets from the Climate Data Store, you need to
> agree with the corresponding data license. This agreement can only be done online.
{: .callout}

Let's look at the default selected boxes:
- **Product type**: Monthly averaged reanalysis by hour of day
- **Variable**: Total precipitation
- **Year**: 2003
- **Month**: June
- **Time**: 06:00
- **Format**: NetCDF 

Please note that it is always good practice to select a small sample of data (in the present instance we take only one month) to check that it meets your needs!

Another issue here may be that apart from the variable and date, all the other boxes ticked involve notions that we do not understand yet..

## What is 2m total precipitation?

We selected [ERA5 monthly averaged data on single levels from 1979 to present](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=form) so we expected to get surface variables only.

In fact, we get all the variables on a single level and usually close to the surface (for example the *2m temperature* is computed as the temperature at a reference height at 2 metres).

## Data format: GRIB versus NetCDF

### GRIB

[GRIB](https://en.wikipedia.org/wiki/GRIB) (GRIdded Binary or General Regularly-distributed Information in Binary form)

### NetCDF

[NetCDF](https://en.wikipedia.org/wiki/NetCDF)

## The Climate Data Store toolbox

In this section, we will briefly introduce the Climate Data Store toolbox.

### "Show Toolbox request" 

{% include links.md %}

