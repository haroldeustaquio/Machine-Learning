# Water Temperature Prediction Using Oceanographic Data (CalCOFI Dataset)

## Project Overview

This project aims to predict **water temperature** using oceanographic data from the **CalCOFI** dataset. The dataset contains various oceanographic measurements such as salinity, oxygen levels, and depth. The objective is to explore whether water temperature can be predicted accurately using regression models, specifically **Linear Regression** and **Lasso Regression**.

## Problem Statement

The goal is to predict the **water temperature** based on other variables provided in the dataset. A high level of accuracy is desired to demonstrate the effectiveness of these regression models in predicting environmental data.

## Dataset

The dataset used is the **CalCOFI "bottle" dataset**, which includes measurements collected from oceanographic stations in the Pacific Ocean. Key variables include:

- **T_degC**: Water temperature (target variable)
- **Salnty**: Water salinity.
- **O2ml_L**: Oxygen concentration.
- **Depthm**: Water depth.
- **O2Sat**: Oxygen saturation percentage.
- **STheta**: Potential density of the water.
- **more cols**

## Data Preparation

The data preparation steps include:

1. **Loading and Exploring the Data**: The dataset is loaded and an initial exploration is performed.
2. **Data Cleaning**: Columns with a high percentage of missing values are removed, as well as irrelevant columns. Remaining rows with missing values are also removed.
3. **Feature Selection**: Columns that are not relevant to the model are dropped, and the dataset is cleaned for further analysis.

## Model Building and Training

The data is split into training and testing sets. Two regression models are used:

- **Linear Regression**
- **Lasso Regression**

## Model Evaluation

The models are evaluated using the following metrics:

- **R² Score**: Proportion of variance explained by the model.
- **Root Mean Squared Error (RMSE)**: Measures the average magnitude of the error.
- **Mean Absolute Error (MAE)**: Average absolute difference between predicted and true values.

## Results

The evaluation metrics for each model are collected and compared to determine the best performing model.

## Conclusion

This project successfully demonstrates the prediction of water temperature using oceanographic variables. The **Linear Regression** model achieved an R² score of approximately 1 (0.99), indicating a near-perfect fit to the data, which is more accurate compared to the **Lasso Regression** model. This suggests that Linear Regression is more effective for this particular dataset in predicting water temperature.
