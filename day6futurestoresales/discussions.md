QUESTIONS AND DISCUSSIONS:

EDA :

there is upward trend in no of passengers over years
the pattern is seasonal and there are peaks and drops in each year almost at same time interval

STATIONARITY TESTING

A stationary time series is one whose statistical properties (mean, variance, autocorrelation) do not change over time.

IT IS IMPORTANT FOR TIME SERIS MODELS BECAUSE THE MODELS ASSUME DATA IS STATIONARY
NON STATIONARY DATA CAN GIVE MISLEADING RESULTS ANS POOR MODEL PERFORANCE

ADF TEST
The Augmented Dickey-Fuller (ADF) test on the original 'Passengers' data resulted in a p-value of 0.991880. Since this p-value is much greater than 0.05, we fail to reject the null hypothesis. This indicates that the original time series is non-stationary

EFFECT OF LOG TRANSFORMATION ⁉

applying log transformations stabalised variance of time seris data
the p value is decreased to be optimum i.e <0.05
while log transformation is a crucial step for this dataset to stabilize variance, it's the combination with differencing that effectively reduced the p-value towards stationarity.

ARIMA MODEL PERFORMANCE

Based on the high p-value of the ADF test on the original data (which would likely still be high after just a log transformation), a non-seasonal ARIMA model without differencing would not be expected to perform well on the log-transformed data. ARIMA models rely on the data being stationary after the specified differencing, and if it's not, the model's assumptions are violated, leading to poor forecasts. The SARIMA model is expected to perform better because it explicitly accounts for seasonality.

