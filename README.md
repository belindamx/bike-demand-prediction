# Bike-Share Demand Prediction

## Overview
Build and evaluate machine learning models to predict hourly bike rental demand for Seoul's bike-share program using structured time series data and engineered temporal features. 

Dataset: Seoul Bike Sharing dataset (UCI Machine Learning Repository)

## Models
- Linear Regression  
- Feedforward Neural Network (FFNN)  
- Gradient Boosted Trees (XGBoost)  

## Key Features
- Cyclical encoding (hour, day of year)  
- Lag features (1 hour, 24 hours)  
- Rolling mean (3-hour window)  
- Weather and seasonal variables  

## Results
XGBoost achieves the best performance across all metrics:

| Model               | MAE  | RMSE | R²    |
|---------------------|------|------|-------|
| Baseline            | 535  | 645  | 0.00  |
| Linear Regression   | 327  | 438  | 0.54  |
| FFNN                | 326  | 446  | 0.53  |
| XGBoost (Validation)| 118  | 198  | 0.91  |
| XGBoost (Test)      | 96   | 145  | 0.94  |