# Fake Bills Detecter

In this project, I performed logistic regression analysis using two different approaches to handle missing values: *without Iterative Imputer* and with *Iterative Imputer*.

## Dataset Overview

The dataset consists of **1500 rows** and **7 columns**. The columns are as follows:

- **is_genuine**: boolean
- **diagonal**: float
- **height_left**: float
- **height_right**: float
- **margin_low**: float
- **margin_upper**: float
- **length**: float

## Data Source

The data was sourced from the following Kaggle dataset:

**[Fake Bills Dataset](https://www.kaggle.com/datasets/alexandrepetit881234/fake-bills/data)**

## Algorithms

### Logistic Regression without Iterative Imputer

In the first approach, I utilized logistic regression without any imputation method to handle missing data. The results indicated that the model was able to achieve a good performance, but it might not have been optimal due to the presence of missing values in the dataset.

### Logistic Regression with Iterative Imputer

In the second approach, I applied *Iterative Imputer* to handle the missing values before fitting the logistic regression model. This method allowed for a more sophisticated estimation of missing values, resulting in improved model performance. The learning curves demonstrated that:

- In one scenario, the validation curve was slightly higher than the training curve, suggesting good generalization capabilities of the model.
- In another scenario, the training curve was above the validation curve, but both curves were convergent, indicating a reasonable balance between fitting the training data and generalizing to unseen data.

Overall, the use of *Iterative Imputer* provided a significant enhancement to the logistic regression analysis, leading to better model performance and more reliable predictions.

## Conclusion

The analysis highlights the importance of handling missing data effectively. The application of *Iterative Imputer* not only improved the model's performance but also facilitated a convergence in the learning curves, demonstrating the model's ability to generalize well across different scenarios.

## How to Run the Project

1. Clone the repository to your local machine.
2. Download the dataset from the [Fake Bills Dataset](https://www.kaggle.com/datasets/alexandrepetit881234/fake-bills/data) and place it in the `data` folder.
3. Ensure all necessary libraries are installed:
    - `pandas`
    - `matplotlib`
    - `sklearn`
    - `seaborn`
    - `numpy`
