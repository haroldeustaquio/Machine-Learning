# Weather Data During World War II - Analysis Project

## Dataset Overview

This project explores the weather data collected during World War II, which can be found on Kaggle: [WeatherWW2 Dataset](https://www.kaggle.com/datasets/smid80/weatherww2/data). The data contains detailed information on weather conditions recorded at various weather stations around the world. These include temperature, precipitation, snowfall, wind speed, and other weather-related metrics.

The primary objective of this analysis is to understand weather patterns and explore how they influenced historical events, like military operations, by building machine learning models that predict maximum temperature (`MaxTemp`) based on other weather conditions.

---

## Project Structure

1. **Data Loading and Exploration**
   - The dataset is loaded using `pandas`, and initial exploration is performed with `.info()` and `.isna().sum()` to check for missing values and understand the structure of the dataset.

2. **Data Cleaning and Preparation**
   - Unnecessary columns such as `STA`, `Date`, `YR`, and several others are dropped to streamline the dataset.
   - The `Snowfall` column is cleaned by handling the invalid `#VALUE!` entries and converting the data type to `float`.
   - Rows with missing values are removed to ensure model accuracy.

3. **Data Scaling/Normalization**
   - Before model building, the dataset is normalized to ensure proper feature scaling.
   - Correlation between variables is visualized using `seaborn.heatmap()` to identify the strongest relationships, such as between `MinTemp`, `MeanTemp`, and `MaxTemp`.

4. **Model Building**
   - Two linear regression models (`LinearRegression` and `Lasso`) are built using `scikit-learn`. 
   - The dataset is split into training and test sets using `train_test_split()`.

5. **Model Evaluation**
   - Both models are evaluated using various regression metrics:
     - **R² Score** (`r2_score`)
     - **Root Mean Squared Error** (`mean_squared_error`)
     - **Mean Absolute Error** (`mean_absolute_error`)
   - These metrics help compare the performance of each model on the test set.

---

## Libraries Used

- **pandas**: For data manipulation and cleaning.
- **seaborn**: For data visualization (correlation heatmap).
- **scikit-learn**: For model building, splitting data, and evaluation metrics.
  - `LinearRegression`
  - `Lasso`
  - `train_test_split`
  - `r2_score`, `mean_squared_error`, `mean_absolute_error`
