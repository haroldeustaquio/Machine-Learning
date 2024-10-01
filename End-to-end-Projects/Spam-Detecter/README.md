# Spam Email Classification Project

## Overview

This project involves classifying emails as spam or non-spam using various Machine Learning models. The objective is to evaluate and compare the performance of different algorithms and vectorization techniques, including Decision Trees, Logistic Regression, SVM, and Naive Bayes. Metrics such as accuracy, precision, recall, and F1 score are used for assessment.

## Objectives

1. **Evaluate Different Models:** Assess the performance of machine learning algorithms including Decision Trees, Logistic Regression, SVM, and Naive Bayes.
2. **Compare Vectorization Techniques:** Test text vectorization methods such as CountVectorizer and TfidfVectorizer.
3. **Analyze Performance Metrics:** Use accuracy, precision, recall, and F1 score to determine model effectiveness.
4. **Optimize Models:** Identify the best-performing models and vectorization techniques based on the results.

## Models and Techniques

- **Naive Bayes:**
  - Vectorization: CountVectorizer, TfidfVectorizer

- **Decision Trees:** 
  - Criteria: Entropy, Gini, Balanced
  - Vectorization: CountVectorizer, TfidfVectorizer

- **Logistic Regression:** 
  - Optimization Methods: newton-cg, Balanced
  - Vectorization: CountVectorizer, TfidfVectorizer

- **SVM:**
  - Vectorization: CountVectorizer
  - Kernel: Linear


## Key Findings

- **Decision Trees** with the Gini criterion and CountVectorizer achieved high precision (0.851) and an F1 score of 0.760, though with long training times.
- **Logistic Regression** with TfidfVectorizer and the newton-cg method provided a good balance between precision (0.718) and recall (0.811), with relatively short training times.
- **Naive Bayes** with TfidfVectorizer showed high accuracy (0.997198) but had a lower recall compared to Logistic Regression.
- **SVM** with CountVectorizer and a linear kernel showed poor performance with very low precision (0.006) but high recall (0.986).

## Results

The project demonstrates the importance of selecting the appropriate model and vectorization technique for the given problem. Decision Trees and Logistic Regression provided the best balance between precision and recall, while Naive Bayes performed well in terms of accuracy. SVM was less effective in this context.
