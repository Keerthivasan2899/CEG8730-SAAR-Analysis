# CEG8730 – Spatial Analysis of Standard Average Annual Rainfall (SAAR)

## 1. Project Overview

This project investigates the spatial distribution of Standard Average Annual Rainfall (SAAR) across the River Eden Catchment. It combines GIS-based spatial interpolation with statistical analysis to examine the relationship between rainfall, elevation and geographic location.

## 2. Project Objectives

- Examine the spatial distribution of rainfall across the study area.
- Apply and compare IDW, Empirical Bayesian Kriging (EBK) and Spline interpolation methods.
- Investigate the relationship between SAAR and elevation using linear regression.
- Develop simple and multiple linear regression models.
- Estimate rainfall at an ungauged location and assess prediction uncertainty.

## 3. Data

The analysis uses rainfall observations from 24 rain gauge locations, including:

- Standard Average Annual Rainfall (SAAR).
- Elevation (metres).
- Easting and Northing coordinates (British National Grid).

The supporting CSV and metadata files are included in this repository.

## 4. Methodology

### Spatial Analysis
Three interpolation techniques were applied:

- Inverse Distance Weighting (IDW)
- Empirical Bayesian Kriging (EBK)
- Spline interpolation

The resulting rainfall surfaces were visualised in GIS and compared.

### Statistical Analysis
Python and the Statsmodels library were used to perform:

- Exploratory data analysis.
- Simple linear regression (SAAR and elevation).
- Multiple linear regression (SAAR, elevation, easting and northing).
- Residual and normal Q-Q diagnostic analysis.
- Multicollinearity assessment using Variance Inflation Factor (VIF).
- Prediction at an ungauged location with a 95% prediction interval.

## 5. Repository Contents

| File / Folder | Description |
|---|---|
| `CEG8730_SAAR_Statistical_Analysis.ipynb` | Jupyter Notebook containing the statistical analysis |
| `SAAR_elevation.csv` | Rain gauge observations and predictor variables |
| `SAAR_metadata.txt` | Supporting dataset metadata |
| `IDW_SAAR_Map.png` | IDW interpolation result |
| `EBK Reg Pred_SAAR_Map.png` | EBK interpolation result |
| `Spline_SAAR_Map.png` | Spline interpolation result |
| `multiple_diagnostics.png` | Multiple regression diagnostic plots |
| `simple_diagnostics.png` | Simple regression diagnostic plots |
| `multicollinearity_VIF.csv` | VIF results |
| `regression_summaries.txt` | Regression model summaries |

Additional prediction and cross-validation outputs are also included.

## 6. Accessing the Notebook

The Jupyter Notebook can be viewed directly on GitHub or downloaded and opened using Jupyter Notebook or Visual Studio Code with the Python and Jupyter extensions installed.

Required Python libraries include:

- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scipy
- scikit-learn

## 7. Study Area

River Eden Catchment, Cumbria, United Kingdom.

---

**Module:** CEG8730 – Data Analysis and Geographic Information Systems  
**Project:** Spatial Analysis of Standard Average Annual Rainfall (SAAR)
