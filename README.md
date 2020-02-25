# Air_passengers_forecasting
1)     Convert the Dataset into Time Series
This is used to convert the numeric column of dataset into time series object
2)     Analyze the Time Series Object
Decompose the time series into various components.
 
3)     Stationarize a Time Series
In order to build a time series model, we first have to make the series stationary. A stationary series is one whose mean and variance is constant over time. To stationarize a time series we need to perform below steps:

Series Transformation: we can transform the series using boxcox() function. The function stabilizes the variance in the series. Lambda(l) is the parameter of boxcox() function and its value decides what kind of transformation is required for the series.
 
4)     Check Stationarity of Time Series
We need to perform augmented Dickey-Fuller test to check the stationarity of newly transformed series.
5)     Create ACF and PACF Plots
ACF (Auto Correlation Function) and PACF (Partial Auto Correlation Function) are very useful in time series as they help us decide the appropriate time series model for forecasting.
6)     Choose a Time Series Model
I.	ARMA Model
II.	ARIMA Model
III.	SARIMA Model
7)     Build the ARIMA Model Using Different Combinations of ACF and PACF Values
Pick the model with least AIC value, where AIC stands for Akaike Information Criterion, which is a function to determine the best model. Lower the AIC is better the model.
8)     Forecast the Data as per the Above Model
Here we forecast the data as per the model which has been chosen in the above step.
9)     Merge Actual and Forecast in One Series
Here we Merge both Actual and Forecasted data into one series to proceed into next step.
10)     Remove Transformation from Series
Now you have the data series with actual numbers and forecast for next 12 months
