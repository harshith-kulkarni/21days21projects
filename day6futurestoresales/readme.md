# Future Store Sales Forecasting - Time Series Analysis

This project analyzes and forecasts monthly airline passenger numbers using classical time series modeling techniques. The workflow demonstrates key concepts in time series analysis, including stationarity testing, transformations, ARIMA/SARIMA modeling, and model evaluation.

## Project Structure

- `day6futurestoresales.ipynb`: Main Jupyter notebook with all code, analysis, and discussion.

## Steps Performed

1. **Data Loading & Visualization**
   - Loaded the airline passenger time series dataset.
   - Visualized the data to observe trends and seasonality.

2. **Exploratory Data Analysis (EDA)**
   - Identified an upward trend and strong seasonality in passenger numbers.
   - Noted recurring peaks and drops at similar intervals each year.

3. **Stationarity Testing**
   - Used the Augmented Dickey-Fuller (ADF) test to check for stationarity.
   - Found the original series to be non-stationary (p-value ≈ 0.99).

4. **Variance Stabilization & Differencing**
   - Applied log transformation to stabilize variance.
   - Used differencing on the log-transformed data to remove trend and achieve stationarity.
   - Confirmed stationarity with a reduced p-value (< 0.05) after transformation and differencing.

5. **Modeling**
   - **ARIMA Model:** Built a non-seasonal ARIMA(1,1,1) model on log-transformed data.
   - **SARIMA Model:** Built a seasonal SARIMA(1,1,1)(1,1,1,12) model to explicitly capture seasonality.

6. **Model Evaluation**
   - Compared ARIMA and SARIMA forecasts on the test set (1959-1960).
   - Calculated RMSE for both models:
     - ARIMA RMSE: 0.2893
     - SARIMA RMSE: 0.1092
   - SARIMA significantly outperformed ARIMA, highlighting the importance of modeling seasonality.

7. **Discussion & Insights**
   - **Stationarity:** Essential for time series models; non-stationary data leads to poor forecasts.
   - **Log Transformation:** Stabilizes variance but must be combined with differencing for full stationarity.
   - **Model Choice:** SARIMA is superior for seasonal data, as shown by lower RMSE.
   - **Next Steps:** Explore different SARIMA orders, try other evaluation metrics, and back-transform forecasts for interpretability.

## How to Run

1. Open `day6futurestoresales.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells in order to reproduce the analysis and results.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scikit-learn

Install requirements with:
```sh
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn