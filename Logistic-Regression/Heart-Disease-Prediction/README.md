# Heart Disease Prediction

## Project Overview

According to the World Health Organization, an estimated **12 million deaths** occur worldwide every year due to heart diseases. In the United States and other developed countries, cardiovascular diseases account for half of all deaths. Early prognosis of cardiovascular diseases can aid in making decisions regarding lifestyle changes for high-risk patients, ultimately reducing complications.

This research aims to identify the most relevant risk factors for heart disease and predict the overall risk using logistic regression.

## Data Source

The data was sourced from the following Kaggle dataset:

**[Heart Disease Prediction Dataset](https://www.kaggle.com/datasets/naveengowda16/logistic-regression-heart-disease-prediction)**

## Methodology

In this project, I employed three different imputation techniques to handle missing values:

1. **KNN Imputer**
2. **Simple Imputer**
3. **Iterative Imputer**

After preprocessing the data with these imputers, I applied logistic regression using the `liblinear` solver both with balanced and unbalanced classes for each of the three cases.

### Conclusion

The best performance was achieved using the `liblinear` solver with `balanced` classes. Importantly, this success was contingent on processing the missing values with the *Iterative Imputer*, which provided a distinct advantage over the other types of imputation methods.

## How to Run the Project

1. Clone the repository to your local machine.
2. Download the dataset from the [Heart Disease Prediction Dataset](https://www.kaggle.com/datasets/naveengowda16/logistic-regression-heart-disease-prediction) and place it in the `data` folder.
3. Ensure all necessary libraries are installed:
    - `pandas`
    - `matplotlib`
    - `sklearn`
    - `seaborn`
    - `numpy`

## Acknowledgements

This project draws upon datasets and research provided by the World Health Organization and other reputable sources on cardiovascular health.
