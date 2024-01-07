# EasyDataPy
EasyDataPy is a unofficial Python library to read in data from EasyData platform of the State Bank of Pakistan

# Where to find details about EasyDataPy
https://pypi.org/project/EasyDataPy/

# About the Library/Package
This package is intended to identify a session with EasyData API key, obtain information about a particular series of interest, and download a series of interest to Python for further analysis. Although, I could have performed basic time-series in Python such as:

1.Plotting the time-series 
2. Unit-Root tests 
3. Seasonality tests 
4. Cointegration tests and Cointegrated vector autoregressive model 
5. Autoregressive and Vector Autoregressive models 
6. Forecasting using Machine Learning and Dynamic Factor models (Rolling and Fixed Window Forecast) 
7. In and Out-of-Sample Forecasts

But this package is not intended to conduct these analysis but I am programming another one, which will be able to perform all of these operations. Stay Tuned!

# How to install and use
Inside the Python you just need to type "pip install EasyDataPy"

# How to use the functions inside this library/package

# Verifying EasyData API Key
EasyData_key_setup("C10D3D29160CE5693F56AA9846ABB2C423D8B123") <- type in/paste your EasyData API Key!

# Finding if the EasyData API Key has been verified
session_has_key()

# Getting the entered key for further use
get_Easydata_key()

# Downloads Weighted-average Overnight Repo Rate series as a Pandas dataframe
data_frame = download_series("TS_GP_IR_REPOMR_D.ORR", "2015-05-25" ,"2023-12-20", "csv")

# Tranforming output of download_series function, that is object called data_frame into a usable time-series
build_time_series(data_frame)

# Plot Time-Series Graph for the downloaded time-series
plot_time_series(data_frame)
