## Model Card

### Model Description

**Input:** The input is a time series of monthly champagne sales data.

**Output:** The output is the model's forecasted sales figures for future months.

**Model Architecture:** The model used is SARIMA (Seasonal Autoregressive Integrated Moving Average), specifically SARIMA(1, 1, 1)x(1, 1, 1, 12).

### Performance

We measured the model's performance by assessing its ability to predict future sales figures. We used metrics such as Mean Absolute Error (MAE) and Mean Squared Error (MSE) for evaluation. The model performed well in capturing seasonal trends.

### Limitations

• The model's predictions are based solely on historical data and may not account for external factors affecting sales.
• Seasonal patterns can change over time, and the model may not adapt to rapid shifts.
• The dataset used for training is relatively small, limiting the model's ability to capture complex trends.

### Trade-offs

• While SARIMA is effective for seasonal time series data, it may struggle with highly irregular data patterns.
• The model might not generalise well to other sales datasets with different characteristics.
• Frequent model retraining may be necessary to capture evolving seasonal patterns.
