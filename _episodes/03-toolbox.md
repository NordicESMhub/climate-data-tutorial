---
title: "Climate Data Store Toolbox"
teaching: 0
exercises: 0
questions:
- "How to download ERA5 and/or CMIP5?"
- "What Essential Variables can I download from ERA5 and/or CMIP5?"
- "How to use CDS API and CDS Toolbox?"
- "What is the best workflow to analyze and visualize CMIP data?"
objectives:
- "Get an overview of various aspects of CMIP5"
- "Learn about Earth System Grid Federation (ESGF)"
- "Learn how to manipulate netCDF data"
- "Learn how to work with CMIP data"
- "Learn how to work with ERA5 data"
keypoints:
- "CMIP5 Essential Information"
---

Let's look at the default selected boxes:
- **Product type**: Monthly averaged ensemble members
- **Variable**: 2m temperature
- **Year**: 2019
- **Month**: June
- **Time**: 00:00
- **Format**: NetCDF 

Please note that the year, month and time may be different (depends on the current date when the request is done!).

And apart from the date, all the other default values introduce notions we do not understand yet!

### What is an ensemble?

Ensemble modelling is a method used to give an indication of the range of possible future states of the Earth (here the atmosphere). 
Instead of making one single simulation, a set (or ensemble) of simulation is produced. 

Multiple simulations are run, each with a slight variation of its initial conditions and with slightly perturbed models. These variations represent the inevitable uncertainty in the initial conditions and approximations in the models. They produce a range of possible values.

### What is a member?

A member from an ensemble simulation is one single simulation among the set of perturbed runs. To ease identification, we give a number to each of the perturbed runs.

So for instance the member 0 is usually associated to what we call the control run e.g. the simulation has not been perturbed.


When selecting "Monthly averaged ensemble members" of ERA 5 data as *Product type* and one variable and date only, you will get 10 different fields covering the entire globe. 

ERA5 provides an estimate of uncertainty through the use
of a 10-member ensemble of data assimilations (EDA) at a
coarser resolution (63 km horizontal resolution) and 3-hourly
frequency.


### How to use ensemble simulations?

Downloading ensemble simulations is useful to get an indication of the variability of a particular parameter and for statistical analysis.

## What is 2m temperature?

We selected [ERA5 monthly averaged data on single levels from 1979 to present](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=form) so we expected to get surface variables only.

In fact, we get all the variables on a single level and usually close to the surface. Here *2m temperature* is computed as the temperature at a reference height (2 metres).

## Data format: GRIB versus NetCDF

### GRIB

[GRIB](https://en.wikipedia.org/wiki/GRIB) (GRIdded Binary or General Regularly-distributed Information in Binary form)

### NetCDF

[NetCDF](https://en.wikipedia.org/wiki/NetCDF)

{% include links.md %}

