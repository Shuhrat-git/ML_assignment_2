# Aquifer Depth Prediction Project

This project aims to predict the **depth to groundwater** based on past data about rainfall, temperature, drainage, and river hydrometry, using **Random Forest Regression**.

## Project Overview

- **Objective:** Predict groundwater depth for month K using data from months K, K-1, ..., K-12.
- **Data:** Aquifer time series dataset.
- **Target variable:** `depth_to_groundwater_m`

## Pipeline

1. **Data loading and inspection.**
2. **Time-based interpolation to fill missing values.**
3. **Monthly aggregation using median values.**
4. **Creation of lagged features (K to K-12 months).**
5. **Model training with RandomForestRegressor.**
6. **GroupKFold cross-validation to avoid leakage.**
7. **Model evaluation with R2 score and RMSE.**
8. **Actual vs Predicted plot visualization.**

## Model Information

- **Model input size:** 52 features
- **Model output size:** 1 target value
- **Cross-validation folds:** 5
- **Cross-validation groups:** Year of each sample
- **Evaluation metrics:** R2 Score, RMSE

## Keywords covered

- model input size
- model output size
- preprocessing
- scaling
- model
- predict
- cross-validation folds
- cross-validation groups
- evaluation metric

---
