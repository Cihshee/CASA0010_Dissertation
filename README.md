# The Conditional Effects of Transport Accessibility on the London Rental Market

**Author:** Yiyao Cui
**Programme:** MSc Urban Spatial Science
**Institution:** The Bartlett Centre for Advanced Spatial Analysis, University College London [cite: 1]
**Date:** August 22, 2025
**Supervisor:** Dr. Roberto Murcio

---

## Abstract

Transport accessibility is a critical determinant of urban property values, yet its precise impact on the rental market, particularly for non-motorized travel modes, remains underexplored. Existing research often relies on simplistic distance metrics and overlooks the conditional nature of accessibility's influence across different segments of the housing market. This dissertation addresses these gaps by investigating the non-linear and conditional relationship between accessibility and housing rents in London.

Using a comprehensive dataset of property listings from 2017 to 2024, this study calculates granular walking and cycling accessibility to London underground stations via the r5r routing package. It also employs a multi-model approach, combining Quantile Regression to analyze effects across different market segments and an interpretable LightGBM machine learning model to capture complex, non-linear dynamics. The findings reveal that walking and cycling accessibility are primary predictors of rental prices in London. The relationship is significantly non-linear, with a rental premium that peaks not immediately adjacent to a station but at a short distance of approximately five minutes, after which the effect diminishes. Furthermore, the analysis demonstrates that this accessibility premium is conditional, with a substantially greater effect on higher-priced properties than on their lower-priced counterparts.

The results offer valuable evidence for policy makers and urban planners concerned with housing affordability, transport equity, and the potential for transport-induced gentrification.

---

## Repository Content

This repository contains the data and R scripts used for the analysis in this dissertation. The file structure is organized as follows:

- **`/data/`**: This directory contains the raw and processed data used in the study.
  - `london_property_listings_2017_2024.csv`: The complete dataset of property listings.

- **`/code/`**: This directory contains the R scripts and Python scripts for the entire analysis workflow.
  - `01_data_preprocessing.R`: Script for cleaning, preparing, and spatially joining the raw property data.
  - `02_accessibility_calculation.R`: Script that uses the `r5r` package to calculate walking and cycling travel times from each property to the nearest underground stations.
  - `03_quantile_regression.R`: Script for running the Quantile Regression models to analyze effects across different market segments.
  - `04_lightgbm_model.R`: Script for training, testing, and interpreting the LightGBM machine learning model.
  - `05_visualizations.R`: Script to generate the plots, maps, and figures used in the dissertation.


- **`README.md`**: This document.

