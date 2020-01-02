# Lasso regression with Random Forests feature selection

This model is designed to predict the final selling price of a given house 
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview/description

### Stage 1 - feature selection
we select all features that have an eigenvalue greater than 0.001. Thus we retain over 95% of our predictive power, and reduce the number of features in our dataset drastically.

### Stage 2 - prediction
using only the features we identified in (1), we predict selling price with Lasso regression. Model also uses cross validation, to give greatest confidence that we aren't overfitting.

Final accuracy is 90.7%
