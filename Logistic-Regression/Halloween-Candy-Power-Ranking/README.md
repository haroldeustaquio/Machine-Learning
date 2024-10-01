# Halloween Candy Power Ranking

## Dataset

The dataset, titled **The Ultimate Halloween Candy Power Ranking**, can be found [here](https://www.kaggle.com/datasets/fivethirtyeight/the-ultimate-halloween-candy-power-ranking). It includes the following attributes for each candy, along with its ranking:

- **chocolate**: Does it contain chocolate? (1 = Yes, 0 = No)
- **fruity**: Is it fruit flavored? (1 = Yes, 0 = No)
- **caramel**: Is there caramel in the candy? (1 = Yes, 0 = No)
- **peanutalmondy**: Does it contain peanuts, peanut butter, or almonds? (1 = Yes, 0 = No)
- **nougat**: Does it contain nougat? (1 = Yes, 0 = No)
- **crispedricewafer**: Does it contain crisped rice, wafers, or a cookie component? (1 = Yes, 0 = No)
- **hard**: Is it a hard candy? (1 = Yes, 0 = No)
- **bar**: Is it a candy bar? (1 = Yes, 0 = No)
- **pluribus**: Is it one of many candies in a bag or box? (1 = Yes, 0 = No)
- **sugarpercent**: The percentile of sugar it falls under within the dataset.
- **pricepercent**: The unit price percentile compared to the rest of the set.
- **winpercent**: The overall win percentage according to the 269,000 matchups.

## Methodology

To predict whether a candy is chocolate or not, I used logistic regression with the following parameters:

- **Solver**: `lbfgs`
- **Regularization Parameter (C)**: 0.5

### Results

The model achieved the following performance metrics:

- **Precision**: 1.0
- **F1 Score**: 0.8421
- **Recall Score**: 0.7273

These results indicate that the model is highly effective at predicting chocolate candies, achieving perfect precision while maintaining a reasonable balance between recall and F1 score.

## Conclusion

This analysis highlights the effectiveness of logistic regression in classifying candy types based on various attributes. The findings can provide insights into consumer preferences and the characteristics that make certain candies more desirable during Halloween.

## How to Run the Project

1. Clone the repository to your local machine.
2. Download the dataset from the [Ultimate Halloween Candy Power Ranking Dataset](https://www.kaggle.com/datasets/fivethirtyeight/the-ultimate-halloween-candy-power-ranking) and place it in the `data` folder.
3. Ensure all necessary libraries are installed:
    - `pandas`
    - `sklearn`
    - `seaborn`
    - `numpy`
