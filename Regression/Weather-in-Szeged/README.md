# Weather in Szeged 2006-2016

## Overview

This project investigates the relationship between humidity and temperature, and apparent temperature, using weather data from Szeged between 2006 and 2016. The primary objective is to determine if there is a significant relationship between these variables and to predict the apparent temperature based on humidity.

## Dataset

The dataset [Szeged Weather Dataset](https://www.kaggle.com/datasets/budincsevity/szeged-weather) used in this project contains the following columns after cleaning:

- `Formatted Date`: Date of the weather observation.
- `Summary`: Weather summary (e.g., clear, cloudy).
- `Precip Type`: Type of precipitation (e.g., rain, snow).
- `Temperature (C)`: Temperature in Celsius.
- `Apparent Temperature (C)`: Apparent temperature in Celsius.
- `Humidity`: Relative humidity percentage.
- `Wind Speed (km/h)`: Wind speed in kilometers per hour.
- `Wind Bearing (degrees)`: Wind direction in degrees.
- `Visibility (km)`: Visibility distance in kilometers.
- `Pressure (millibars)`: Atmospheric pressure in millibars.

Note: Columns `Loud Cover` and categorical columns were dropped due to lack of variance or non-numeric data.

## Data Cleaning and Preparation

1. **Import Libraries**: Used libraries include `pandas`, `seaborn`, `sklearn`, and `numpy`.
2. **Load and Explore Data**: Loaded the dataset and explored its structure.
3. **Data Cleaning**: Dropped non-numeric columns and the `Loud Cover` column, as it only contained zero values.
4. **Correlation Analysis**: Visualized the correlation matrix to understand relationships between variables.

## Model Building and Training

Two regression models were used to predict the temperature:

1. **Linear Regression**
2. **Lasso Regression**

### Metrics

The following metrics were computed to evaluate the models:

| Model            | R² Score | RMSE   | MAE    |
|------------------|----------|--------|--------|
| Linear Regression | 0.990    | 0.951  | 0.743  |
| Lasso            | 0.989    | 0.988  | 0.765  |

- **R² Score**: Measures the proportion of variance in the dependent variable that is predictable from the independent variables.
- **RMSE (Root Mean Squared Error)**: Measures the average magnitude of the errors in the predictions.
- **MAE (Mean Absolute Error)**: Measures the average magnitude of the errors in the predictions, without considering their direction.

