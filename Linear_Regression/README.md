
# Linear Regression

A machine learning project implementing linear regression from scratch and comparing it with scikit-learn's implementation.

## Overview

This notebook demonstrates:
- Building a linear regression model using gradient descent
- Computing cost function and gradients manually
- Training on a dataset from Kaggle
- Comparing custom implementation with scikit-learn

## Dataset

Uses the [Random Linear Regression dataset](https://www.kaggle.com/datasets/andonians/random-linear-regression) from Kaggle.

## Key Functions

- `compute_cost()` - Calculates Mean Squared Error
- `compute_gradient()` - Computes gradients for weight and bias
- `linear_regression()` - Implements gradient descent optimization
- `predict()` - Generates predictions
- `measure()` - Evaluates MSE and RMSE

## Models Trained

1. **Custom Implementation** - Gradient descent with 10,000 iterations and learning rate 1.0e-4
2. **Scikit-learn** - Built-in LinearRegression for comparison

## Results

The notebook trains both models on 80% of the data and evaluates on 20% test set, visualizing the regression fit.

## Requirements

- numpy
- matplotlib
- scikit-learn
- kagglehub
- pandas
