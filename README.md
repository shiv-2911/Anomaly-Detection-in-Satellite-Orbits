# Anomaly Detection in Satellite Orbits
## Orbit Data Analysis Using ARIMA, VARIMA, XGBoost, and CatBoost

This repository implements anomaly detection in satellite orbits using advanced time-series modeling and machine learning techniques. The project leverages ARIMA, VARIMA, XGBoost, and CatBoost models to analyze satellite Two-Line Element (TLE) data and detect deviations caused by maneuvers.

### Key Functionalities:
* **Data Handling:**
  - Imports and preprocesses TLE data for various satellites.
  - Handles missing or duplicate entries, ensuring data consistency.
* **Exploratory Data Analysis (EDA):**
  - Generates visualizations and statistical summaries of orbital elements.
  - Produces time-series plots with maneuver indicators for intuitive analysis.
* **Anomaly Detection:**
  - Implements ARIMA models to forecast orbital elements and detect anomalies through residual analysis.
  - Utilizes VARIMA (Vector AutoRegressive Integrated Moving Average) for multivariate time-series analysis.
  - Applies XGBoost and CatBoost models for machine-learning-based anomaly detection.
* **Model Optimization:**
  - Tunes ARIMA and VARIMA parameters (p, d, q) for optimal time-series forecasting.
  - Optimizes XGBoost and CatBoost hyperparameters using grid search or random search.
  - Evaluates model performance using metrics like Mean Squared Error (MSE), precision, and recall.
* **Advanced Features:**
  - Identifies and visualizes anomalies with maneuver overlays on time-series plots.
  - Provides detailed comparison of model performance across various techniques.
  - Quantitatively measures the performance of the model using matching techniques to find maneuvers.

### Data Source:
- The script processes TLE data files and maneuver records. Ensure these files are placed in the appropriate directory or update paths in the script accordingly.

### Requirements:
- **Python 3.x** and the following libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - statsmodels
  - xgboost
  - catboost
  - scikit-learn
