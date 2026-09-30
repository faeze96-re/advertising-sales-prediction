# Advertising Sales Prediction

## Overview

This project uses the Advertising dataset to analyze the relationship between advertising expenditure and sales.

The main goal is to build a multiple linear regression model to predict Sales using TV and Radio advertising expenditure.

## Dataset

The dataset contains advertising expenditure in:

- TV
- Radio
- Newspaper

The target variable is:

- Sales

## Project Steps

- Data exploration
- Missing value and duplicate checking
- Correlation analysis
- Exploratory data visualization
- Multicollinearity analysis using VIF
- Statistical analysis using OLS
- Feature selection
- Multiple linear regression
- Model evaluation
- Residual analysis
- Cross-validation

## Feature Selection

OLS results were used to examine the statistical significance of the predictors.

Newspaper was excluded from the final regression model because its coefficient was close to zero and its p-value was high.

The final model uses:

- TV
- Radio

## Model Evaluation

The model is evaluated using:

- R²
- Adjusted R²
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy
