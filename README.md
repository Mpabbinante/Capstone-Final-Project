# Capstone-Final-Project
## Analyzing Time Series Data with Python

This Python code demonstrates the analysis of time series data using various methods from the `statsmodels` library.

## Libraries Used

python
-import os
-import pandas as pd
-import matplotlib.pyplot as plt
-from statsmodels.tsa.arima.model import ARIMA
-from datetime import datetime, timedelta
-import numpy as np
-from statsmodels.tsa.holtwinters import ExponentialSmoothing
-from statsmodels.tsa.api import VAR
-from statsmodels.tsa.statespace.varmax import VARMAX
-from statsmodels.tools.eval_measures import rmse
-from statsmodels.tsa.vector_ar.vecm import coint_johansen
# 1. Data Loading and Preprocessing
Data Source: Average_sale_price_us_houses.csv
Steps:
Loaded the dataset using pandas.
Processed the data for analysis.
Set the appropriate datetime index for time series analysis.
Prepared the data for visualization and modeling.
# 2. Exploratory Data Analysis (EDA) and Visualization
Conducted exploratory analysis:
Displayed initial insights into the trends of average sale prices and yearly changes in housing prices over time.
Utilized matplotlib to create time series plots showcasing the trends.
# 3. Moving Average Analysis
Calculated and visualized 5-year moving averages to identify long-term trends in the data.
Analyzed how the moving averages compared to actual trends in average sale prices and yearly changes.
# 4. ARIMA Model for Forecasting
Utilized the ARIMA (AutoRegressive Integrated Moving Average) model for forecasting future trends in:
Average Sale Price(year)
Yearly Change in Average Sale Price
Fitted the ARIMA models and generated forecasts for the next 10 years based on historical data.
# 5. Holt-Winters Exponential Smoothing
Applied Holt-Winters Exponential Smoothing to predict future trends in:
Average Sale Price(year)
Yearly Change
Utilized the technique to generate forecasts for the upcoming 10 years.
# 6. Forecasted Values and Statistics
Presented the forecasted values and basic statistics derived from the ARIMA and Holt-Winters models:
Displayed the forecasted trends for average sale prices and yearly changes in housing prices.
Calculated statistical measures (mean, standard deviation, minimum, maximum, percentiles) for the forecasted data.