# Forecasting the Return on Investment (ROI) for a House in Melbourne: A Five-year Sales Analysis

This project is used for forecasting the ROI of new home clusters that will be constructed in the next year in Melbourne by taking past data such as reviews, prices, etc.

The details of this project could be accessed through this document:
[Problem Identification.pdf](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/Problem%20Identification/%5BREPORT%20-%20BDA%5D%20Forecasting%20the%20Return%20on%20Investment%20(ROI)%20for%20a%20House%20in%20Melbourne_A%20Five-year%20Sales%20Regression%20Analysis.pdf)

## Dataset

[Melbourne Housing Market](https://www.kaggle.com/datasets/anthonypino/melbourne-housing-market?select=Melbourne_housing_FULL.csv)

[Cleaned Melbourne Housing Market](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/1.%20Data%20Pre-Processing/MELBOURNE_CLEANED_DATASET.csv)

## Project Structure

This project is will implementing Cross Industry Standard Process for Data Mining (CRISP - DM), which includes:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Deployment

However, we wil separate it into several phases as follows:

- [Data Preprocessing](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/1.%20Data%20Pre-Processing/Data%20Preprocessing.ipynb)
- [Checking the OLS Assumptions](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/2.%20OLS%20Assumptions/OLS%20Assumptions.ipynb)
- [Dummy Variables](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/3.%20Dummy%20Variables/Dummy%20Variables.ipynb)
- [Modeling](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/4.%20Modeling/Modeling.ipynb)

### Data Preprocessing

1. Data Cleaning
2. Data Reduction

### Modeling

1. [Multi Linear Regression](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/tree/main/Multiple%20Linear%20Regression)
2. [Neural Network](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/Neural%20Network/Neural%20Network.ipynb)

## Conclusion

We could say that the data is not well-suited for regression analysis, and this issue indicates that the data is not linear. You could see the result of this dataset analysis in [here](https://github.com/iannn07/S5-BDA-Project-House-ROI-Forecasting/blob/main/4.%20Modeling/Modeling.ipynb).

While using the Neural Network, we obtain better results in its accuracy by looking at its MSE, MAE, and RMSE. However, there's something unique in this Regression Analysis: the R-Squared. Below is the summary result of both models:

| Performance Measure | Multiple Linear Regression | Neural Network     |
| ------------------- | -------------------------- | ------------------ |
| R-Squared           | 0.5926448818238725         | 0.5237713739630026 |
| MSE                 | 1.2604419499246601e+26     | 84018888704.0      |
| MAE                 | 579344653273.0378          | 192391.421875      |
| RMSE                | 11226940589157.227         | 289860.11920234904 |

Thus, in short the best model for this data is a non-linear model.
