# stocks-prediction
## Dataset

The stock prediction model is trained on a dataset containing historical market data. Here is a sample snippet of the dataset:

| Date         | Open    | High    | Low     | Close   | Shares Traded    | Turnover (₹ Cr)  |
|--------------|---------|---------|---------|---------|------------------|------------------|
| 09-NOV-2015  | 7788.25 | 7937.75 | 7771.70 | 7915.20 | 218,422,388.0    | 9,376.17         |
| 10-NOV-2015  | 7877.60 | 7885.10 | 7772.85 | 7783.35 | 170,267,413.0    | 7,153.47         |
| 11-NOV-2015  | 7838.80 | 7847.95 | 7819.10 | 7825.00 | 22,380,435.0     | 1,123.44         |
| 13-NOV-2015  | 7762.45 | 7775.10 | 7730.90 | 7762.25 | 165,876,819.0    | 7,731.55         |
| 16-NOV-2015  | 7732.95 | 7838.85 | 7714.15 | 7806.60 | 154,134,885.0    | 6,871.15         |
| 17-NOV-2015  | 7848.75 | 7860.45 | 7793.00 | 7837.55 | 149,451,211.0    | 6,367.14         |

*Note: This is just a sample; the full dataset includes additional rows and columns.*

## Model Performance

Here are the evaluation metrics for the multi-output regression models used in the stock prediction project. The target variables include 'High', 'Low', and 'Close' prices, and the models predict all three simultaneously:

### Random Forest Regressor (RFR):
- **Mean Squared Error (MSE):** 8803.88
- **Mean Absolute Error (MAE):** 64.37
- **R-squared (R²):** 0.9994

### Support Vector Regression (SVR):
- **Mean Squared Error (MSE):** 12148547.63
- **Mean Absolute Error (MAE):** 2756.34
- **R-squared (R²):** 0.1315

### Linear Regression (LR):
- **Mean Squared Error (MSE):** 6100.61
- **Mean Absolute Error (MAE):** 55.10
- **R-squared (R²):** 0.9996

### Gradient Boosting Regressor (GBR):
- **Mean Squared Error (MSE):** 7850.66
- **Mean Absolute Error (MAE):** 62.68
- **R-squared (R²):** 0.9994

- ## Best Performing Model

After thorough evaluation of the regression models, the Random Forest Regressor (RFR) has demonstrated superior performance in predicting 'High', 'Low', and 'Close' stock prices based on historical market data. The evaluation metrics for RFR are as follows:

- **Mean Squared Error (MSE):** 8803.88
- **Mean Absolute Error (MAE):** 64.37
- **R-squared (R²):** 0.9994

These metrics indicate that the Random Forest Regressor provides the most accurate predictions compared to other models.

### Why Random Forest Regressor?

The Random Forest Regressor excels in capturing complex relationships in the data, which is crucial for accurate stock price predictions. Its ensemble learning approach, combining multiple decision tree regressors, allows it to handle non-linear patterns and outliers effectively.
