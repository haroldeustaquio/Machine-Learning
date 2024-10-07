# Boston Housing Price Prediction with Decision Trees and Ensemble Methods

This repository contains a project that predicts housing prices in the Boston area using Decision Tree Regression and various ensemble methods. The project includes data preprocessing, model training, hyperparameter tuning using GridSearchCV, and evaluation of the performance of multiple models, including Decision Tree Regressor, Random Forest, Bagging Regressor, AdaBoost, Gradient Boosting, and XGBoost.

## Project Overview

This project focuses on predicting the median value of owner-occupied homes (`MEDV`) in the Boston area. While Decision Tree Regressor is one of the models used, the project also explores ensemble methods to improve the predictive accuracy. Models such as Random Forest, Bagging, AdaBoost, Gradient Boosting, and XGBoost are evaluated and compared.

## Dataset

The dataset used in this project is the [Boston Housing dataset](https://www.kaggle.com/datasets/arslanali4343/real-estate-dataset), which includes various features such as crime rate, average number of rooms per dwelling, and more. The target variable (`MEDV`) represents the median value of owner-occupied homes in $1000s.

**Dataset Source:** The dataset is originally from the UCI Machine Learning Repository but can also be found in other machine learning libraries like `sklearn`.

### Features in the Dataset

- **CRIM:** Per capita crime rate by town.
- **INDUS:** Proportion of non-retail business acres per town.
- **NOX:** Nitric oxide concentration (parts per 10 million).
- **RM:** Average number of rooms per dwelling.
- **AGE:** Proportion of owner-occupied units built before 1940.
- **DIS:** Weighted distances to five Boston employment centers.
- **TAX:** Property tax rate per $10,000.
- **PTRATIO:** Pupil-teacher ratio by town.
- **B:** Proportion of the population that is African-American.
- **LSTAT:** Percentage of lower status of the population.
- **MEDV:** Median value of owner-occupied homes in $1000s (Target Variable).

## Models Used

This project evaluates multiple models to improve the prediction accuracy, including:

- **DecisionTreeRegressor:** A simple decision tree model.
- **Random Forest Regressor:** An ensemble method that builds multiple decision trees and averages their predictions.
- **Bagging Regressor:** A model that reduces variance by training multiple trees on different subsets of data.
- **AdaBoost Regressor:** A boosting method that combines weak learners to create a stronger model.
- **Gradient Boosting Regressor:** Another boosting method that optimizes model performance iteratively.
- **XGBoost:** An optimized implementation of gradient boosting that is often faster and more accurate.

## Setup

To run this project, you need to have Python installed along with the following libraries:

- `pandas`
- `scikit-learn`
- `xgboost`
