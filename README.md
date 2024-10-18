# PJM East Electricity Demand Forecasting with Prophet

This repository demonstrates time series forecasting for electricity demand using the PJM East dataset and the **Prophet** library. The goal is to train a model to predict electricity usage and evaluate its performance.

## Overview
This project performs time series forecasting on the PJM East electricity demand dataset using Prophet, a popular library for forecasting that supports trends, seasonality, and holidays. 

## Dataset
The dataset used is the **PJM East Electricity Demand** dataset, which contains hourly data for electricity usage measured in megawatts (MW). 

- `Datetime`: Timestamp of the data
- `PJME_MW`: Electricity demand in MW

### Model Training
We split the dataset into training and testing sets based on a cut-off date (`1-Jan-2015`) and train the Prophet model on the training data. The test set is used to evaluate the model's performance.

### Forecasting and Evaluation
We use the trained model to predict future electricity demand and compare the predictions against the actual values. Several metrics, such as RMSE, MAE, and MAPE, are calculated to evaluate the model's performance.

### Holidays Integration
The project also includes an analysis of the impact of US Federal Holidays on the forecast accuracy. We incorporate holidays into the Prophet model.

## Results
- Visualizations include the forecast vs. actual values and a zoomed-in view for specific dates, such as the first week of January 2015.
- Holiday impact analysis shows the effect of holidays (e.g., July 4th) on electricity demand.

## Metrics
We calculate the following error metrics to evaluate the performance of the model:

- **RMSE (Root Mean Squared Error)**: Measures the average magnitude of the forecast error.
- **MAE (Mean Absolute Error)**: Captures the average absolute error between predicted and actual values.
- **MAPE (Mean Absolute Percentage Error)**: Provides a percentage-based error metric.

