Hourly Taxi Demand Forecasting Using Time Series Models
In this project, I analyzed historical taxi order data collected by Sweet Lift Taxi to predict the number of taxi orders for the next hour during peak demand periods at airports.

The data was resampled to an hourly frequency and explored to identify daily and weekly seasonality patterns, including rush-hour peaks. To capture temporal dependencies, I engineered time-based features such as lag values, rolling statistics (means and standard deviations), and calendar features (hour of day, day of week, weekend indicators).

The dataset was split chronologically, reserving the last 10% as a test set while using the remaining data for training and validation with time series cross-validation. Several models were evaluated, including a naïve baseline, Ridge Regression, and Random Forest.

The Random Forest model with tuned hyperparameters delivered the best performance, achieving a test RMSE of approximately 43.1, outperforming both the naïve baseline (≈ 58.9) and Ridge Regression (≈ 47.1). While extreme spikes were slightly under-predicted, the model successfully captured overall demand trends and seasonal patterns.

This solution can help the company anticipate demand more accurately and strategically allocate drivers during peak hours, improving service efficiency and customer satisfaction.
