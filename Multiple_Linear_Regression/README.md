# Multiple Linear Regression

This project implements multiple linear regression from scratch using gradient descent and compares it with scikit-learn's implementation.

## Overview

The notebook demonstrates:
- Building a multiple linear regression model using gradient descent
- Training and testing on student performance data
- Comparing custom implementation with scikit-learn's `LinearRegression`

## Dataset

Uses the [Student Performance](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression) dataset from Kaggle, predicting Performance Index based on multiple features.

## Implementation Details

### Custom Model
- **Algorithm**: Gradient Descent
- **Features**: 4 input features (excludes Extracurricular Activities and target)
- **Iterations**: 50,000
- **Learning Rate**: 0.0001

## Accuracy Comparison

The custom gradient descent model may show slightly lower accuracy than scikit-learn due to:

| Method | Approach | Convergence |
|--------|----------|-------------|
| Custom GD | Iterative optimization | Requires multiple iterations to converge |
| Sklearn | Normal Equations | Solves directly in one operation (closed-form solution) |

Scikit-learn uses **Normal Equations**, which compute optimal weights analytically without iteration, achieving exact results faster. The gradient descent approach requires careful tuning of learning rate and iterations to reach similar accuracy.