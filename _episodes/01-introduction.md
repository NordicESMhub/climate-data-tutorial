---
title: "Introduction"
teaching: 0
exercises: 0
questions:
- "What is climate Data?"
- "Where to get climate data?"
objectives:
- "Learn terminology about Climate data"
- "Get an overview of the various Climate data offering"
- "Learn to understand Climate data, climate projections"
- "Learn to understand Climate Data Formats"
- "The Earth System Grid Federation (ESGF)"
- "The Copernicus Climate Data Store (CDS)"
keypoints:
- "Climate data"
- "netCDF"
- "GRIB"
- "CMIP"
- "Copernicus"
- "ESGF"
- "CDS"
---

# What is climate?

Go to [www.menti.com](https://www.menti.com/) and use the code given by your instructor.

According to https://en.wikipedia.org/wiki/Climate
Climate is defined as the average state of everyday's weather condition over a period of 30 years. It is measured by assessing the patterns of variation in temperature, humidity, atmospheric pressure, wind, precipitation, atmospheric particle count and other meteorological variables in a given region over long periods of time.
Climate differs from weather, in that weather only describes the short-term conditions of these variables in a given region. 

# Climate terminology

## Climate prediction vs. projection
A climate prediction (or climate forecast) is an attempt to produce an estimate of the actual evolution of the natural climate in the future, for example, at seasonal, inter-annual or long-term time scales. Since the future evolution of the climate system may be highly sensitive to initial conditions, such predictions are usually probabilistic in nature.
Climate projections are distinct from climate predictions in that projections depend upon emission/concentration/radiative forcing scenarios, which are based on assumptions concerning, for example, future socio-economic and technological developments that may or may not be realized and are therefore subject to substantial uncertainty.

## Climate change modelling
Climate models are a mathematical representation of the climate developed by scientists to understand and predict the climate system. In order to be able to do this, the models divide the earth, ocean and atmosphere into a grid. The values of the predicted variables, such as surface pressure, wind, temperature, humidity and rainfall are calculated at each grid point over time, to predict their future values.
Various types of models are used to analyse different aspects of the climate. If the natural system is altered by assuming socio-economic trends, greenhouse gas emissions, or other activities by man, the climate models project future climates. These projections are scenarios of how man’s activities may affect the natural climate.

## Different types of models
There are many types of numerical climate models which differ by their complexity and coupling between various components (from more or less simplified atmosphere only models, to models where the atmosphere is coupled with land and/or ocean, and now full Earth system models including biogeochemistry, hydrology, land use, etc.). 

<img src="../fig/ClimateModelsEvolution.gif">
(from https://www.giss.nasa.gov) As computing power has increased since the 1970s, so has the complexity of the computer models used to simulate Earth's climate. Most of the time indicual components are developed separately and later coupled into more complex and comprehensive models which are then finely "tunned" so that the result is in line with the observed climate.

The models broadly fall into these categories:
* Global/General Climate/Circulation Models (GCM) and Earth System Models (ESM), which simulate the climate of the entire planete (generally with a coarse spatial resolution);
* Regional Climate Models (RCM), which focus on a limited area of the world (generally with a fine resolution);
* Variable Resolution Models (VR-Models), which use a coarse grid for the global domain and a variable horizontal mesh refinement over a region of interest:

<img src="../fig/EUCordex30x4.png">

## Observations (or observational data)
These are measurements (from ground stations, buoys, satellites, etc.) of the occurrence of one or more physical variables (temperature, humidity, wind, etc.) at one or more particular times and places in and on the atmosphere, ocean, etc. 

Observations can be direct or indirect:
* direct when a physical parameter is measured directly, for example temperature or pressure at a land station: 

<img src="../fig/WMO Global Observing System.png">
(from https://uls.climate.copernicus.eu) The sensors themselves can be either in-situ (hence providing information about their immediate environment) or remote (in which case they are able to measure over distances that extend significantly beyond the location of the instrument itself).

* indirect when they are derived from other observations, for example information related to past climate (these are sometimes referred to as "climate proxies") can be inferred from tree rings (dendrochronology), lake sediments (varves) or ice cores.

<img src="../fig/frost_rings_375.jpg">
(from https://www.earth.columbia.edu) Example taken from a Siberian pine tree in Mongolia where the distorted rings are evidence of a drastic cooling in the northern hemisphere (due to a massive volcanic eruption) that froze sap in the cells during the growing season in years 536-537 C.E. 

## Reanalyses
A new reanalysis product (called ERA5) has recently been released by ECMWF as part of Copernicus Climate Change Services. This product has higher spatial resolution (31 km) and covers the period from 1979 to present (and this will soon be extended to 1950).
In addition to re-analysing all the old data using a consistent system, the reanalyses also make use of much archived data that was not available to the original analyses. This is because in a weather centre only data arrived before the model runs start can be used, also not all the huge volume of satellite data can be processed and used, for obvious operational constraints, however they could have been of great value to improve the forecasting. This allows for corrections to be made at a later stage as well as filling gaps in areas where data was sparse. 

> ## Note: 
> Some people erroneously call reanalysis products “gridded observational data” as if by some magic trick observations not
> made in the first place could be reinvented! Remember that there are values at each grid point and time only because a numerical
> weather prediction model was used and that this model only used the available measurements.

# Climate versus Weather?

> # What is the difference between weather and climate?
>
> This exercise is meant to be done in small groups (2-3 persons).
> Take 5 minutes to discuss about the difference between weather
> and climate. 
> Summarize your discussions in the workshop etherpad.
>
> {: .challenge}

See [Video](https://youtu.be/e0vj-0imOLw) as a summary/solution of the preceding exercise.

# What do we mean by climate data?

## Essential Climate Variables

## Exercices

# Where can we get Climate data?

## 

{% include links.md %}

