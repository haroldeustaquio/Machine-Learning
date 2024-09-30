# Predicting MBTI Personality Types

This project aims to predict the Myers-Briggs Type Indicator (MBTI) personality types using a synthetic dataset from Kaggle. The dataset includes over 100,000 samples and contains demographic information, interest areas, and personality scores that help determine an individual's MBTI type.

## Data Source

The data was sourced from the following Kaggle dataset:

**[Predict People Personality Types Dataset](https://www.kaggle.com/datasets/stealthtechnologies/predict-people-personality-types)**

### Dataset Description

This synthetic dataset is designed to explore and predict MBTI personality types based on a combination of demographic factors, interest areas, and personality scores. It includes the following features:

- **Age**: A continuous variable representing the age of the individual.
- **Gender**: A categorical variable indicating the gender of the individual ('Male' or 'Female').
- **Education**: A binary variable where a value of 1 indicates the individual has at least a graduate-level education (or higher), and 0 indicates an undergraduate, high school level, or uneducated.
- **Interest**: A categorical variable representing the individual's primary area of interest.
- **Introversion Score**: A continuous variable (0-10) representing the individual's tendency toward introversion versus extraversion (higher scores indicate a greater tendency toward extraversion).
- **Sensing Score**: A continuous variable (0-10) representing the individual's preference for sensing versus intuition (higher scores indicate a preference for sensing).
- **Thinking Score**: A continuous variable (0-10) indicating the individual's preference for thinking versus feeling (higher scores indicate a preference for thinking).
- **Judging Score**: A continuous variable (0-10) representing the individual's preference for judging versus perceiving (higher scores indicate a greater preference for judging).
- **Personality**: The target variable containing the MBTI personality type.

## Methodology

To predict the MBTI personality type, a **Logistic Regression** model was used. Multiple solver configurations and class weight options were tested to identify the best-performing model based on metrics such as accuracy, F1 score, precision, and recall.

### Trained Models

The following variants of the **LogisticRegression** model were trained:

| Model                                     | Accuracy | F1 Score | Precision | Recall   |
|-------------------------------------------|----------|----------|-----------|----------|
| LogisticRegression - newton-cg - None     | 0.826076 | 0.822679 | 0.821617  | 0.826076 |
| LogisticRegression - newton-cg - balanced | 0.764518 | 0.778458 | 0.815118  | 0.764518 |
| LogisticRegression - sag - None           | 0.172597 | 0.168800 | 0.165290  | 0.172597 |
| LogisticRegression - sag - balanced       | 0.117364 | 0.122100 | 0.160197  | 0.117364 |
| LogisticRegression - saga - None          | 0.175044 | 0.170186 | 0.165811  | 0.175044 |
| LogisticRegression - saga - balanced      | 0.135974 | 0.148503 | 0.166727  | 0.135974 |
| LogisticRegression - lbfgs - None         | 0.187303 | 0.175951 | 0.167419  | 0.187303 |
| LogisticRegression - lbfgs - balanced     | 0.112054 | 0.131062 | 0.165167  | 0.112054 |

Each of these configurations was tested to determine which was most suitable for this dataset and prediction task.

## Conclusion

The results clearly demonstrate the importance of selecting the appropriate solver and class balancing technique for logistic regression models. The most effective model is **Logistic Regression with the Newton-CG solver and without balanced class weighting**, achieving an impressive accuracy of **82.61%** and an **F1-score of 0.82**. This model strikes a solid balance between precision and recall, making it highly effective for overall classification tasks.

In contrast, the second-best model, which also uses the Newton-CG solver but with balanced weighting, underperforms slightly with an **F1-score of 0.78**. While this suggests it may be less prone to overfitting, it does not surpass the unbalanced Newton-CG variant.

Models using the **Sag, Saga, and Lbfgs** solvers—both with and without balanced weighting—consistently showed poor performance, with accuracies around **11-17%**, indicating their unsuitability for this particular dataset. These findings emphasize the critical role of choosing the right solver and balancing technique when implementing logistic regression models.

## How to Run the Project

1. Clone the repository to your local machine.
2. Download the dataset from the [MBTI Dataset](https://www.kaggle.com/datasets/stealthtechnologies/predict-people-personality-types) and place it in the `data` folder.
3. Ensure all necessary libraries are installed:
    - `pandas`
    - `matplotlib`
    - `sklearn`
    - `seaborn`
