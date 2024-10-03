# Iris Classification using Decision Tree Classifier

## Project Overview

This project implements a **Decision Tree Classifier** to classify the famous **Iris dataset**. We explore two different criteria for splitting the nodes in the decision tree: **Gini Index** and **Entropy**. The objective is to compare the performance of these two methods and observe how they influence the accuracy and general performance of the model.

### Dataset

The Iris dataset consists of 150 samples of flowers, divided into three species: Setosa, Versicolor, and Virginica. Each sample contains four features:

- **Sepal Length**
- **Sepal Width**
- **Petal Length**
- **Petal Width**

These features are used to classify the species of the flower.

### Model: Decision Tree Classifier

We have implemented a Decision Tree Classifier from the `sklearn` library. Two different splitting criteria were explored:

1. **Gini**
2. **Entropy** (information gain)

Both methods aim to maximize the purity of the nodes in the decision tree, but they do so through different mathematical approaches. Despite these differences, both methods yielded similar results on this dataset.

### Results

After training the classifier using both **Gini** and **Entropy**, the models performed similarly in terms of accuracy and confusion matrix:

- **Accuracy**: High accuracy was achieved in both cases, with slight variation between the methods.
- **Confusion Matrix**: Both models effectively classified the Iris species, with minimal confusion between Versicolor and Virginica classes.
