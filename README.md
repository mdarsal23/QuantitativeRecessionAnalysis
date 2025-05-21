# QuantitativeRecessionAnalysis
This Repository holds the model for quantitative recession analysis 
This project was offered by the Econs Society, IIT Kanpur.
# Scope of Project
To forecast the probability of a recession using macroeconomic indicators
# Key Indicators
Yield curve (10-year minus 2-year Treasury spread)
Unemployment rate (U-3)
Industrial Production / Manufacturing PMI
Real GDP growth
Consumer Sentiment / Retail Sales
# Data
The data for this project is collected from FRED (Federal Reserve of Economic Data)
# Feature Engineering
All the datapoints with NA are dropped and three lags are created for current data to apply time series effectively
At the end of this step model is left with 10 coloumns with 8 coloumns as regressors 
Yield spread and Unemployment have 3 extra coloumns of Lag 1, 3, 6.
The data is finally normalised (mean = 0, variance = 1) for better fitting
# Model Selection and Training
The model used is Logistic Regression and end result is probability of recession happening in the next time period given current situations.
Accuracy is 90%
