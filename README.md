# TimeSeriesAnalysis-ARIMA-Model-Comparisons-for-Currency-Conversion-Rates
We will again analyze the currency exchange data but to a greater extent and including two different currencies for comparison

For this data analysis, you will again analyze the currency exchange data but to a greater extent and including two different currencies for comparison. File DailyCurrencyData.csv  Download DailyCurrencyData.csvcontains the daily exchange rate of USD/EUR and USD/GDP from January 1999 through December 31st 2020. File MonthlyCurrencyData-1.csv  Download MonthlyCurrencyData-1.csvMonthlyCurrencyData.csv contains the monthly exchange rate of USD/EUR and USD/GDP for the same time period. Similarly to homework 2, we will aggregate the daily data into weekly data. We will compare our analysis using ARMA modeling on both weekly and monthly data for the two currencies.



Question 1. Weekly vs Monthly Exploratory Data Analysis (20 points)

1a. Based on your intuition, when would you use weekly vs monthly time series data?

1b. Plot the time series plots for both currency exchange rates comparing weekly vs monthly data. How do the weekly and monthly time series data compare? How do the time series for the two currencies compare?

1c. Fit a non-parametric trend using splines regression to both the weekly and monthly time series data for both currencies. Overlay the fitted trends for each of the currency separately. How do the trends compare when comparing those fitted using the weekly and monthly data? How do the trends for the two currencies compare?

1d. Take the 1st order difference of the time series weekly vs monthly data. Plot the ACF plots and compare. How do the difference time series for weekly and monthly data compare in terms of stationarity? How do the difference time series for the two currencies compare in terms of serial dependence and stationarity?

Question 2. ARIMA Fitting and Forecasting: Weekly Data Analysis (23 points)

2a. Divide the data into training and testing data set, where the training data exclude the last eight weeks of data (November and December 2020) with the testing data including the last eight weeks of data. For both currency exchange rates and using the training datasets, use the iterative model to fit an ARIMA(p,d,q) model with max AR and MA orders of 8,  and a differencing order of 1 or 2. Display the summary of the final model fit. Compare statistical significance of the coefficients. Would a lower order model be suggested based on the statistical significance of the coefficients?

2b. Evaluate the model residuals using the ACF and PACF plots, the residual plot and residuals' histogram as well as hypothesis testing for serial correlation for the selected models in (2a) for the two currencies.  Does the model fit the time series data? Compare the model fit for the two currency exchange rates.

2c. For each currency exchange, apply the model identified in (2a) and forecast the last eight weeks of data. Plot the predicted data to compare the predicted values to the actual observed ones. Include 90% confidence intervals for the forecasts in the corresponding plots.

2d. Calculate Mean Absolute Percentage Error (MAPE) and Precision Measure (PM). How many observations are within the prediction bands?  Compare the accuracy of the predictions for the two time series using these two measures. 

Question 3. ARIMA Fitting: Monthly Data Analysis (17 points)

3a. Divide the data into training and testing data set, where the training data exclude the last two months of data (November and December 2020) with the testing data including the last two months.  For both currency exchange rates and using the training datasets, use the iterative model to fit an ARIMA(p,d,q) model with max AR and MA orders of 8,  and a differencing order of 1 or 2. Display the summary of the final model fit. Compare statistical significance of the coefficients. Compare the order selection from using monthly versus weekly data for each of the two currencies.

3b. For each currency exchange, apply the model identified in (3a) and forecast the last two months of data.  Plot the predicted data to compare the predicted values to the actual observed ones. Include 90% confidence intervals for the forecasts in the corresponding plots. 

3c. Calculate Mean Absolute Percentage Error (MAPE) and Precision Measure (PM). How many observations are within the prediction bands?  Compare the accuracy of the predictions for the two time series using these two measures. 

Question 4.  Weekly vs Monthly Forecasting  (5 points)

Compare the forecasts based on the weekly versus monthly data. Overlay the forecast into one single plot for each of the two currency exchange rates. What can you say about using weekly versus monthly data?

Question 5. Reflection on ARIMA (5 points)

Considering your understanding of the ARIMA model in general as well as what your understanding of the behavior of the currency exchange data based on the completion of the above questions, how would you personally regard the effectiveness of ARIMA modelling? Where would it be appropriate to use it for forecasting and where would you recommend against? What are some specific points of caution one would need to consider when considering using it?

 


