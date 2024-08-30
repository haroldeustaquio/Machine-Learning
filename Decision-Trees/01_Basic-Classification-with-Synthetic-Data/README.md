# Basic Classification with Synthetic Data

## Project Description

This mini-project introduces users to the implementation of decision trees, a fundamental algorithm in the field of Machine Learning. By generating and classifying a synthetic dataset, users will learn how to train and evaluate a decision tree model, optimize its hyperparameters, and visualize its internal structure.

## Specific Objectives

1. **Synthetic Data Generation:** Create a dataset using the `make_classification` function from scikit-learn. The dataset will consist of two classes and four features, two of which will be informative and two redundant, providing a structured environment for experimentation.

2. **Model Training:** Train a decision tree using the generated dataset to learn how to correctly classify the two classes. The model's depth and other hyperparameters will be controlled to prevent overfitting.

3. **Decision Tree Visualization:** Visualize the structure of the trained decision tree using the `plot_tree` function from scikit-learn. This visualization helps users understand how the model makes decisions based on the input features.

4. **Model Evaluation:** Evaluate the model's performance using a confusion matrix and calculate its accuracy. This step provides a quantitative measure of the model's effectiveness.

5. **Hyperparameter Optimization:** Use `GridSearchCV` to optimize the decision tree's hyperparameters, such as `criterion`, `max_depth`, `min_samples_split`, and `min_samples_leaf`, to improve the model's accuracy.

## Tools Used

- **Python 3.x**: The programming language used for this project.
- **scikit-learn**: Used for data generation (`make_classification`), model training (`DecisionTreeClassifier`), hyperparameter optimization (`GridSearchCV`), and performance evaluation (`confusion_matrix`, `accuracy_score`).
- **matplotlib**: Used for visualizing the decision tree (`plot_tree`).

## Requirements

- **Python 3.x**
- **Packages:** 
  - `scikit-learn`
  - `matplotlib`

## Usage Instructions

1. Clone the repository: 
   ```bash
   [git clone https://github.com/yourusername/your-repository.git]
