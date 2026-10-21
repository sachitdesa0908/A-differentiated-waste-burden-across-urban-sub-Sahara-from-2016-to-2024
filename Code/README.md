# Code

## Overview

This directory contains the Python notebooks used to investigate the spatial and temporal distribution of unmanaged waste across ten sub-Saharan African cities between 2016 and 2024, and to extend predictive risk mapping to 36 additional cities.

The analyses encompass continuous waste burden modelling, spatial reorganisation, urban predictor relationships, population exposure, and geographic model transferability.

## Directory structure

The code is organised into four subdirectories:

### 1. `Additional_cities/`
- **`Test cities.ipynb`:** Preparation and harmonisation of urban covariates for the 36 additional cities, assessment of similarity with the ten study cities, application of the transferable XGBoost model, and analysis of predicted waste risk, spatial concentration, and population within high-risk areas.

### 2. `Exposure_surface/`
- **`Exposure_surface_generation_2016&2024.ipynb`:** Generation of continuous, mass-preserving waste burden surfaces for each study city in 2016 and 2024, accounting for waste site area, proximity, and overlapping spatial influence.

### 3. `General/`
- **`Waste_trajectories.ipynb`:** Spatial visualisation and comparison of waste site distributions and trajectories across the ten study cities.
- **`Waste_burden.ipynb`:** Analysis of population proximity and exposure to qualifying waste sites, projections of future exposure, and evaluation of the geographic transferability of waste presence models using leave-one-city-out cross-validation.

### 4. `Predictor_analysis/`
- **`Predictor_analysis_SHAP.ipynb`:** Evaluation of urban predictor importance using SHAP, including comparisons across waste presence, persistence, growth, and decline. Additional analyses examine changes in urban characteristics surrounding areas of increasing and declining waste burden.

## Usage and reproducibility

The notebooks were developed primarily in Python using Google Colab, with libraries for spatial analysis, statistical modelling, machine learning, and visualisation, including `geopandas`, `rasterio`, `scikit-learn`, `xgboost`, `shap`, and `matplotlib`.

The notebooks contain city-specific processing steps and may require adjustments to input paths, output directories, and data dependencies before execution. Supporting datasets are organised within the repository's `Data/` directory.
