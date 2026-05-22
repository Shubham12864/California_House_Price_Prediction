# California House Price Prediction

This repository contains a Jupyter notebook that builds a housing price regression model for the California housing dataset.

## Files

- `California_House_price_prediction.ipynb` - end-to-end notebook for loading data, preprocessing, training, evaluation, and visualization.
- `housing.csv` - input dataset used by the notebook.

## Workflow

The notebook performs the following steps:

1. Load the housing dataset.
2. Remove missing values with `dropna()`.
3. Convert categorical features with one-hot encoding.
4. Split the data into training and test sets.
5. Expand features with polynomial terms.
6. Scale the features.
7. Train an `SGDRegressor` model.
8. Evaluate the model with mean squared error and R2 score.
9. Plot actual vs predicted prices.

## Model Notes

- Model used: `SGDRegressor`
- Feature engineering: `PolynomialFeatures` with degree 2
- Scaling: `StandardScaler`
- Evaluation metrics: Mean Squared Error and R2 Score

## Typical Output

The notebook prints model weights, bias, MSE, R2 score, and a few sample predictions.

## How to Run

Open the notebook in VS Code or Jupyter and run the cells from top to bottom.

## Plot

The final visualization compares actual house prices against predicted prices.