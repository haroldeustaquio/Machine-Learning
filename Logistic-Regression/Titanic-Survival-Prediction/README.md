# Titanic Survival Prediction using Logistic Regression

## Context

The sinking of the Titanic was one of the deadliest maritime disasters in history, with over 1,500 passengers losing their lives. This dataset is designed to help predict whether a passenger survived the disaster based on various factors such as age, sex, class, and ticket fare.

[Link to the dataset on Kaggle](https://www.kaggle.com/datasets/brendan45774/test-file)

## Dataset Information

The dataset contains the following columns:

| Column Name   | Description                              |
| ------------- | ---------------------------------------- |
| PassengerId   | Unique ID for each passenger             |
| Survived      | Survival status (0 = No, 1 = Yes)        |
| Pclass        | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name          | Name of the passenger                    |
| Sex           | Gender of the passenger                  |
| Age           | Age of the passenger                     |
| SibSp         | Number of siblings or spouses aboard     |
| Parch         | Number of parents or children aboard     |
| Ticket        | Ticket number                            |
| Fare          | Fare paid for the ticket                 |
| Cabin         | Cabin number (if available)              |
| Embarked      | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

## Machine Learning Model: Logistic Regression

In this project, I used a **Logistic Regression** model to predict survival based on the available features. Here is the code snippet for training and making predictions:
