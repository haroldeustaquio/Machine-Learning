# Fake News Detection

This project aims to experiment with various Machine Learning (ML) models to detect fake news. We will use different classification algorithms and techniques to determine their effectiveness in identifying false information from textual data.

## Project Overview

- **Objective**: Test and compare the performance of different ML models in fake news detection.
- **Data Source**: Dataset [https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset].
- **Models**: Includes models such as Logistic Regression, Decision Trees, Naive Bayes, and SVM.
- **Evaluation**: Model performance will be evaluated based on accuracy, precision, recall, and F1-score.

## Project Structure

- `data/`: Contains the dataset used for training and testing.
- `testing.ipynb`: Jupyter notebooks for experimentation with different models.

## Structure of `testing.ipynb`

### 1. Importing Libraries

Import all necessary libraries required for data manipulation, visualization, and model building.

### 2. Loading and Exploring the Data

Load the dataset and perform an initial exploration:

- Check the structure of the data.
- Display basic statistics and data types.

### 3. Data Cleaning and Preparation

- **Concatenate true and fake news data**: Combine the true and fake datasets.
- **Remove duplicated rows and handle missing values**: Ensure data integrity by removing duplicates and handling any missing data.
- **Delete blank text**: Remove rows where the text field is blank.
- **Add a column named `complete_text`**: Combine relevant text fields into a single column.
- **Delete punctuation**: Clean the text by removing unnecessary punctuation marks.

### 4. Splitting and Vectorizing Data

- **Train-test split**: Split the dataset into training and testing sets.
- **Vectorization**: Convert the text data into numerical form using methodsslike TF-IDF or Count Vectorizer.

### 5. Model Building and Training

- **Naive Bayes**: Train a Naive Bayes model and improve it based on performance.
- **Decision Trees**: Experiment with different criteria (`entropy`, `gini`) for the Decision Tree classifier.
- **SVM**: Train Support Vector Machines with different kernels (`linear`, `sigmoid`).
- **Logistic Regression**: Train a Logistic Regression model with different solvers (`sag`, `newton`).

### 6. Conclusion

Summarize the findings, including model performance and key insights from the experiment.
