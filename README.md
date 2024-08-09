# Anomaly-Detection-in-Satellite-Orbits
## CryoSat-2, Haiyang-2A, Jason-3, Sentinel-6A, SARAL Orbit Data Analysis

This code analyzes the orbital data of multiple satellites: CryoSat-2, Haiyang-2A, Jason-3, Sentinel-6A, and SARAL. It performs various tasks including data import, formatting, exploratory data analysis (EDA), stationarity testing, ARIMA model fitting, and residual analysis.

### Key Functionalities:
* Imports unpropagated element data (CSV format) for each satellite.
* Extracts manoeuvre start and end dates from a separate .txt file.
* Formats column names for consistency.
* Checks for duplicate data entries.
* Calculates and displays the percentage of missing values in the dataset.
* Generates ACF (autocorrelation function) and PACF (partial autocorrelation function) plots to assess time series stationarity.
* Performs Augmented Dickey-Fuller (ADF) test to statistically determine stationarity.
* Conducts exploratory data analysis (EDA) including:
    * Basic information about the dataset (data types, summary statistics)
    * Time series plots for each orbital element
    * Overlaying manoeuvre start dates on the time series plots for visual reference
* Fits an ARIMA model to each orbital element time series to forecast future values.
* Evaluates different ARIMA parameter combinations (p, d, q) using Mean Squared Error (MSE) to find the best-fitting model.
* Plots the residuals of the best ARIMA model with manoeuvre start dates overlaid.

### Data Source:
* The script assumes the data files (CSV and txt) are located in the same directory as the script.
* Update file paths in the read_satellite_data and extract_start_end_dates function calls to point to your specific data source.

### Running the Code:
Ensure you have Python 3 and the required libraries (pandas, numpy, matplotlib, seaborn, statsmodels) installed.
