# Logistic Regression Model for Stock Price Prediction

![GitHub repo size](https://img.shields.io/github/repo-size/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction)
![GitHub contributors](https://img.shields.io/github/contributors/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction)
![GitHub stars](https://img.shields.io/github/stars/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction?style=social)
![GitHub forks](https://img.shields.io/github/forks/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction?style=social)

## Overview

This repository contains a logistic regression model for stock price prediction using historical stock data. The model is built using Python and the scikit-learn library.

## Dataset

The dataset used for this project is stored in [EURUSD_M1.csv](https://github.com/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction/blob/baa798788a83657ad245f55a0694ebfcde82a761/EURUSD_M1.csv) and includes the following columns:

- Date
- Open
- High
- Low
- Close
- Volume

## Features

- **Target**: Binary target variable indicating the direction of stock price movement (1 for price increase, 0 for price decrease).
- **Percentage Return**: Percentage change in the closing price.
- **Lag1-Lag5**: Lagged percentage returns from previous time periods.
- **LagVolume**: Lagged volume data.

## Model Evaluation
The model is evaluated using classification metrics such as precision, recall, and F1-score. The classification report is printed to the console.
```bash
              precision    recall  f1-score   support

           0       0.57      0.64      0.61       548
           1       0.49      0.42      0.45       452

    accuracy                           0.54      1000
   macro avg       0.53      0.53      0.53      1000
weighted avg       0.54      0.54      0.54      1000
```

## Visualization
The last 400 data points are plotted to visualize the predicted buy (green) and sell (red) signals.
![Price Prediction for Last 400 Data Points with 30-Minute Interval](https://github.com/alimirash/Logistic_Regression_Model_for_Stock_Price_Prediction/blob/1486f4a1253724a00cd4df3be64d49de3391d24b/Price%20Prediction%20for%20Last%20400%20Data%20Points%20with%2030-Minute%20Interval.png)
