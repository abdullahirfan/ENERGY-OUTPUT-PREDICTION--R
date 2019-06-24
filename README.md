What is time-series data?
Data that has some variable which changes over the period of time, example of it can be sales, stock prices, weather etc.

What are the four components of time series?
Time series data is affected by 4 main components
1) Trend - Overall change and pattern of the data. Exmaple: Increasing sales with time throughout the year
2) Seasonality - Changes over period of time, periodic changes. Example Sales of warm clothes. Each winter warm clothes increease and sales peak in december, every december.
3) Cyclicity - Seasonality is annual pattern, cyclicity is random patterns example of Recession.
4) Irregularity- Random component of time series data. Which cannot be explained. Example constant price over period of time

What are the conditions needed to perform time series analysis?
Conditions for Time Series: Data has to be stationary, most cases it is not. You need to make it stationary

What is non-stationary data?
If data has the 4 components it means it is not stationary and most times its raw, so you have to make it stationary data.

How do you differentiate from stationary to non-stationary?
Visually, stationary data would be flatish and not show an upward trend as in increasing trend over time.

Stationarity measured through: Mean , variance and co-variance 
Mean: For stationarity: Mean should remain constant over a period of time, at time t & t + 1
Variance: Variance should reamin constant over period of time.
Covariance: should not change with respect to time for i and i+1 term which means Hour =1 and hour= 2 covaraiance should remain the same.

Now that we have defined what time-series is we will define our analysis, data source, approach & evaluation.


The data was taken from http://reports.ieso.ca/public/DemandZonal/ which are the hourly zonal demand for zones and we will include our analysis for the zone of toronto.

#*************************************************************************************************************

 Our Analysis:
Our objective is to find energy output trend of Toronto from Ontario Electricity supply operator based on the quaterly data from 2003 to 2017.
We will perform a Univariate Autoregressive Integrated Moving Average to learn the pattern of OVERALL ENERGY OUTPUT and then perform prediction on test data of next 4 months.


 Our data source:
The data source is www.ieso.ca. There are a total of 59 rows with granuality of one row showing energy output in any quarter of that year. The data has 3 regions so on any given date there can be 3 records (West,Southwest and Toronto). For the sake of simplicity we are just keeping our Analysis to analyze overall energy output in Toronto.

Approach
1) Data Preprocessing & Exploratory Data Analysis (Relevant to Time Series only)
2) Analysis of Assumptions (Stationarity test) & Data transformation to stationary
3) Implementing ARIMA Model
4) Prediction based on ARIMA model 
5) Evaluation (Test vs Expected)
