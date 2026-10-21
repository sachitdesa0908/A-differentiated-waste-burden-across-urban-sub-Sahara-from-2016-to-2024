# A differentiated waste burden across urban sub-Sahara from 2016 to 2024

## Overview

This repository contains the data, code, analytical results, and figures associated with the research manuscript **"A differentiated waste burden across urban sub-Sahara from 2016 to 2024"**.

The study examines how the spatial distribution of unmanaged waste evolved across ten sub-Saharan African cities between 2016 and 2024, investigating how waste accumulation, urban development, and population exposure changed over time. It further evaluates whether the spatial relationships associated with unmanaged waste are transferable across different urban environments, extending predictive risk mapping to 36 additional cities.

The repository provides the underlying waste site observations, urban covariates, analytical scripts, modelling outputs, and supporting figures to promote transparency, reproducibility, and further research into urban waste accumulation and environmental sustainability.

## Study description

The study covers ten cities across sub-Saharan Africa: **Abidjan, Accra, Dakar, Freetown, Johannesburg, Kampala, Kinshasa, Lagos, Maputo, and Nairobi**.

Unmanaged waste sites were mapped for 2016 and 2024 using satellite imagery, with their geographical locations and spatial footprints used to characterise changes in waste accumulation and distribution. These observations were combined with spatially explicit indicators of population distribution, economic activity, infrastructure accessibility, residential informality, and urban morphology.

The analysis examines three interconnected dimensions of unmanaged waste:

1. **Spatiotemporal change:** Characterising changes in waste site occurrence, size, and spatial organisation, including processes of proliferation, consolidation, and intensification.
2. **Urban conditions and spatial drivers:** Investigating how changes in urban characteristics relate to waste emergence, persistence, growth, and decline, and identifying spatial relationships that recur across cities.
3. **Population exposure and geographic transferability:** Estimating changes in population exposure between 2016 and 2024, projecting exposure to 2030, and applying a transferable predictive model to identify potentially high-risk areas across 36 additional cities.

The study combines continuous spatial representations of waste burden with statistical analysis and machine learning to examine how unmanaged waste becomes embedded within developing urban environments.

Together, these analyses investigate whether increasing waste accumulation necessarily translates into greater population exposure and provide a spatial framework for assessing urban sustainability beyond conventional waste generation and collection statistics.

## Repository structure

The repository is organised into four main directories:

### 1. `Code/`

Contains Python scripts used for spatial data processing, modelling, analysis, and visualisation.

- **`Additional_cities/`:** Scripts associated with the geographic transfer of the waste presence model to 36 additional sub-Saharan African cities.
- **`Exposure_surface/`:** Scripts for generating and analysing continuous spatial representations of waste burden from mapped waste sites.
- **`General/`:** Supporting scripts for the broader spatial and temporal analyses.
- **`Predictor_analysis/`:** Scripts for examining relationships between urban covariates and unmanaged waste, including predictor importance and spatial patterns.

### 2. `Data/`

Contains the spatial datasets and associated information used in the study.

- **`Covariates/`:** Urban environmental, demographic, socioeconomic, and infrastructural predictors used in the spatial analyses.
- **`Master/`:** Integrated datasets combining analytical variables (2016 and 2024) and waste exposure for each year (2016 and 2024).
- **`Polygons/`:** Spatial polygon of waste sites for 2016 and 2024.
- **`Sites/`:** Mapped waste sites for 2016 and 2024.

The waste site observations were collected and curated specifically for the study, providing a consistent basis for examining changes in waste distribution between 2016 and 2024.

### 3. `Figures/`

Contains figures associated with the research manuscript.

- **`Manuscript_figures/`:** Main figures illustrating spatial changes in unmanaged waste, urban drivers, geographic transferability, and population exposure.
- **`Supplementary_figures/`:** Additional visualisations supporting the analyses, methodological evaluation, and interpretation of results.

### 4. `Results/`

Contains supporting analytical documents and summaries associated with the study, including spatial patterns of waste, population exposure, forecasting, predictor analysis, and model transferability.

These materials provide additional context for the analytical findings and methodological decisions presented in the manuscript.

## Data availability

Waste site locations and spatial footprints were generated specifically for this study using satellite imagery and manual verification. The datasets cover observations from 2016 and 2024 across the ten study cities.

The repository includes derived urban covariates and analytical datasets used to investigate the spatial and temporal distribution of unmanaged waste. Supporting materials associated with the 36 additional cities are also provided where applicable.

The data and associated scripts are intended to support reproducibility and further investigation of waste accumulation, urban development, and population exposure across sub-Saharan Africa.

## Methodology and reproducibility

The study integrates satellite-derived waste observations, spatially explicit urban covariates, statistical analysis, and machine learning.

The principal analytical components are:

1. **Waste site mapping:** Identification, verification, and delineation of waste sites across ten cities in 2016 and 2024.
2. **Continuous waste burden modelling:** Generation of spatially continuous, mass-preserving waste burden surfaces incorporating site area, proximity, and overlapping spatial influence.
3. **Spatiotemporal analysis:** Assessment of changes in waste site number, size, distribution, and local burden, distinguishing emergence, persistence, growth, decline, and clearance.
4. **Urban predictor analysis:** Evaluation of demographic, economic, infrastructural, and morphological characteristics associated with waste presence and changing local burdens.
5. **Transferable predictive modelling:** Development of an XGBoost waste presence classifier using five urban predictors, with geographic transferability assessed through leave-one-city-out cross-validation.
6. **Geographic risk assessment:** Application of the transferable model to 36 additional cities, including evaluation of predictor similarity and identification of areas with elevated predicted waste presence.
7. **Population exposure modelling:** Estimation of populations within modelled exposure zones surrounding qualifying waste sites, assessment of changes between 2016 and 2024, and projection of exposure to 2030.
8. **Visualisation:** Generation of spatial maps, statistical figures, and comparative analyses illustrating waste accumulation, exposure, and geographic transferability.

### Software and requirements

The analyses were conducted primarily using:

- **Python:** Spatial data processing, statistical analysis, machine learning, population exposure modelling, and visualisation.
- **GIS software:** Spatial data preparation, inspection, and cartographic visualisation.

The relevant scripts are provided in the `Code/` directory. Users should review the required Python packages, input file paths, data dependencies, and output directories before execution.

Individual subdirectories may contain additional documentation describing their analytical workflows and requirements.

## Citation

If you use the data, code, or results from this repository, please cite the associated manuscript:

**Desa, S., Tomkins, M. D., Harris, A., & Huck, J. J.** A differentiated waste burden across urban sub-Sahara from 2016 to 2024. *Manuscript in preparation.*

## Contact

For questions regarding the datasets, analytical methods, or reproducibility of the study, please contact:

**Sachit Desa**  
Department of Geography  
The University of Manchester  
sachit.desa@manchester.ac.uk
