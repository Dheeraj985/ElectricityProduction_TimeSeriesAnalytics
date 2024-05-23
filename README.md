In this project, we aimed to forecast electricity production using historical data from 1985 to 2017 obtained from Kaggle. We observed an upward trend and significant seasonality in the data. We performed initial predictability tests, confirming the data's predictability through approaches like ARIMA and first lag differencing.

We applied several time series forecasting techniques, including:
1. **Two-Level Forecasting**: Combining a quadratic trend and seasonality model with a Moving Average (MA) trailing method for residuals.
2. **Holt-Winters Model**: Utilizing automated selection for error, level, trend, and seasonality components.
3. **ARIMA (Autoregressive Integrated Moving Average)**: Employing the `auto.arima` function to select the best parameters.

We partitioned the dataset into training (1985-2010) and validation (2011-2017) sets. We evaluated models based on Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE). ARIMA outperformed other methods, with the lowest MAPE and RMSE values, making it the most suitable for forecasting.

The final ARIMA model (2,1,1)(0,1,2)[12] was used to forecast electricity production for the year 2018, providing accurate and reliable predictions. The project highlights the effectiveness of ARIMA in handling time series data with trends and seasonality for future forecasting.
