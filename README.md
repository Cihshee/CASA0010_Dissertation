# The Conditional Effects of Transport Accessibility on the London Rental Market

**Author:** Yiyao Cui

**Programme:** MSc Urban Spatial Science

**Institution:** The Bartlett Centre for Advanced Spatial Analysis, University College London

**Date:** August 22, 2025

**Supervisor:** Dr. Roberto Murcio



## Abstract

Transport accessibility is a critical determinant of urban property values, yet its precise impact on the rental market, particularly for non-motorized travel modes, remains underexplored. Existing research often relies on simplistic distance metrics and overlooks the conditional nature of accessibility's influence across different segments of the housing market. This dissertation addresses these gaps by investigating the non-linear and conditional relationship between accessibility and housing rents in London.

Using a comprehensive dataset of property listings from 2017 to 2024, this study calculates granular walking and cycling accessibility to London underground stations via the r5r routing package. It also employs a multi-model approach, combining Quantile Regression to analyze effects across different market segments and an interpretable LightGBM machine learning model to capture complex, non-linear dynamics. The findings reveal that walking and cycling accessibility are primary predictors of rental prices in London. The relationship is significantly non-linear, with a rental premium that peaks not immediately adjacent to a station but at a short distance of approximately five minutes, after which the effect diminishes. Furthermore, the analysis demonstrates that this accessibility premium is conditional, with a substantially greater effect on higher-priced properties than on their lower-priced counterparts.

The results offer valuable evidence for policy makers and urban planners concerned with housing affordability, transport equity, and the potential for transport-induced gentrification.



## Repository Content

This repository contains the data and R scripts used for the analysis in this dissertation. The file structure is organized as follows:

- **`root`**: This directory contains the R scripts and Python scripts for the entire analysis workflow.
  - `data_analysis.ipynb`: for Exploratory Data Analysis (EDA).
  - `regression-full-2024-6030.ipynb`: contains the regression modeling for the full sample dataset.
  - `regression-common-2024-6030.ipynb`: contains the regression modeling for the common sample dataset.
  - `basic_visual.qmd`: for generating basic, exploratory visualizations of the raw and processed data.
  - `accessibility_common_sample_2024.qmd`: to calculating and analyzing transport accessibility metrics for the "common sample" of properties.
  - `accessibility_full_sample_2024.qmd`: to calculating and analyzing transport accessibility metrics for the "full sample" of properties.

- **`/data/`**: Protected and large datasets are not included here and need to be obtained from official channels. This repository only provides a subset of the processed data.
  - `Underground_Stations_latlon.csv`
  - `properties-with-accessibility-common-sample-2024.csv`
  - `properties-with-accessibility-full-sample-2024.csv`

- **`README.md`**: This document.

