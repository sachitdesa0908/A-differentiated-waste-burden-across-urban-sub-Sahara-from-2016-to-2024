# Data

## Overview

This directory contains the spatial datasets used to investigate the distribution and temporal evolution of unmanaged waste across ten sub-Saharan African cities between 2016 and 2024.

The datasets include mapped waste site locations and footprints, urban covariates, and integrated gridded observations used for spatial analysis, predictive modelling, and population exposure assessment.

## Directory structure

The data are organised into four subdirectories:

### 1. `Covariates/`
Contains spatially explicit urban predictors representing demographic, socioeconomic, infrastructural, and morphological characteristics across the study cities. These include population density, night-time light radiance, slum likelihood, infrastructure accessibility, road proximity, and built environment characteristics.

Covariates were harmonised to a common 30 m spatial grid and aligned with the 2016 and 2024 observations where temporally appropriate.

### 2. `Master/`
Contains integrated city-level gridded datasets combining urban covariates with derived waste burden measures. These datasets provide the principal analytical inputs for examining waste presence, spatial change, predictor relationships, and model transferability.

### 3. `Polygons/`
Contains spatial polygon datasets representing the mapped footprints of waste sites across the ten study cities for 2016 and 2024.

These datasets preserve the geographical extent and area of individual waste accumulations, supporting analyses of site size, spatial distribution, and temporal change.

### 4. `Sites/`
Contains city-specific waste site observations, including geographical locations and mapped site areas for 2016 and 2024.

These records support analyses of waste site occurrence, size distributions, spatial clustering, and changes in waste accumulation across cities.

## Data preparation and usage

Waste sites were identified from satellite imagery, individually verified, and manually delineated using high-resolution imagery. The resulting observations were combined with spatially explicit urban covariates to construct harmonised analytical datasets.

The datasets support continuous waste burden modelling, spatiotemporal analysis, machine learning, and population exposure assessment. Associated processing and modelling notebooks are available in the repository's `Code/` directory.


