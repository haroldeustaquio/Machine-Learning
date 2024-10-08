# Car Price Prediction Dataset

This dataset contains various features related to cars, including the year of manufacture, selling price, kilometers driven, fuel type, seller type, transmission type, number of previous owners, mileage, and engine specifications. These attributes provide valuable insights into the factors influencing car prices and can be used to develop predictive models for estimating the selling price of cars.

---

## Source
The dataset is available on Kaggle: [Car Price Prediction Dataset](https://www.kaggle.com/datasets/sukhmandeepsinghbrar/car-price-prediction-dataset)
---
## Features
| Feature                | Description                                          |
|------------------------|------------------------------------------------------|
| **name**               | Name of the car                                      |
| **year**               | The year of manufacture of the car                   |
| **selling_price**      | The selling price of the car in the local currency   |
| **km_driven**          | The total kilometers driven by the car               |
| **fuel**               | The type of fuel used by the car                     |
| **seller_type**        | The type of seller                                   |
| **transmission**       | The transmission type of the car                     |
| **owner**              | The number of previous owners of the car             |
| **mileage (km/ltr/kg)**| The mileage or fuel efficiency of the car            |
| **engine**             | The engine specifications of the car                 |
---
## Models to be Developed
| Model                    | R²        | RMSE      |
|--------------------------|-----------|-----------|
| 2  BaggingRegressor      | 0.958589  | 0.020162  |
| 1  RandomForestRegressor  | 0.958537  | 0.020175  |
| 5  XGBRegressor          | 0.950877  | 0.021959  |
| 0  DecisionTreeRegressor   | 0.932984  | 0.025649  |
| 4  AdaBoostRegressor       | 0.932984  | 0.025649  |
| 3  GradientBoostingRegressor | 0.922036 | 0.027665  |
---
## Libraries to be Used
- **Scikit-learn**: For implementing machine learning algorithms.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Statsmodels**: For statistical modeling.
