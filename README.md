# PG&E Data Analysis and Forecasting

This repository contains scripts for analyzing and forecasting electricity usage and cost data from Pacific Gas and Electric Company (PG&E). The analysis involves data cleaning, preparation, exploratory analysis, and forecasting using the Prophet time series forecasting framework.

### Prerequisites

Ensure you have Python installed on your machine, ideally through Anaconda to manage packages and environments. The following Python libraries are required:
- pandas
- prophet
- matplotlib
- plotly
- numpy
- scikit-learn


### Data
The data used in this project are stored in CSV files:

pge_1.csv: Contains data from 2022-04-24 - 2023-04-23
pge_2.csv: Contains data from 2023-04-23 - 2024-04-05

### Data Cleaning
Data is prepared by:

Merging multiple data sources.
Dropping unnecessary columns and rows.
Converting data types and handling date-time conversions.
Aggregating data on a daily and weekly basis.
Removing Outliers.

###  Exploratory Analysis
Initial data visualization is done using Plotly to plot the daily and weekly trends in usage and cost.

###  Forecasting
The forecasting is performed using the Prophet model, adjusted for:

Yearly and monthly seasonality.
Public holidays.
A regressor for summer months to account for seasonal variations.
Personal Vaccations(Dec - Jan)

### Model Evaluation
The model's performance is evaluated using:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R-squared (R²)
Cross-validation is performed to assess the model's predictive accuracy and generalization capability.

### Predictions
Future predictions are made for the next 52 weeks to analyze expected usage and costs.

<img width="1300" alt="Screenshot 2024-04-13 at 2 54 37 PM" src="https://github.com/PurvaB25/pge_prophet/assets/100107332/5c5e5bd7-38d7-474e-8b8c-454c1b337578">


