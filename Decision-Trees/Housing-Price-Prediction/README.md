# Boston Housing Price Prediction with Decision Trees

This repository contains a project that predicts housing prices in the Boston area using Decision Tree Regression. The project includes data preprocessing, model training, hyperparameter tuning using GridSearchCV, and evaluation of the model's performance.

## Project Overview

This project focuses on predicting the median value of owner-occupied homes (`MEDV`) in the Boston area using a Decision Tree Regressor. The model is trained and evaluated on a modified version of the Boston Housing dataset.

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

## Setup

To run this project, you need to have Python installed along with the following libraries:

- `pandas`
- `scikit-learn`
