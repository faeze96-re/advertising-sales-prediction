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
The initial model included TV, Radio, and Newspaper.
Newspaper was removed from the final model because its coefficient was close to zero and its p-value was high (p ≈ 0.954). Removing Newspaper had almost no effect on R², while Adjusted R² slightly improved.
The final model uses:
- TV
- Radio

## Model Evaluation

The model is evaluated using:

- R²
- Adjusted R²
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
## Results

The final multiple linear regression model uses TV and Radio advertising expenditure to predict Sales.

### Test Set Performance

| Metric | Value |
|---|---:|
| R² | 0.908 |
| MAE | 1.27 |
| MSE | 2.85 |
| RMSE | 1.69 |

The model explains approximately 91% of the variance in Sales on the test set.

### Model Coefficients

The final model uses:

- TV
- Radio

Newspaper was excluded from the final model because its coefficient was close to zero and its p-value was high in the OLS analysis.

### Additional Analysis

- VIF was used to check multicollinearity.
- Residual analysis was performed.
- Shapiro-Wilk test was used to assess residual normality.
- 5-fold cross-validation was performed to evaluate model stability.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy
