# Solar Power Generation Prediction

Machine learning project that predicts the AC power output of a solar plant's inverters from weather sensor data.

## Problem
Solar output changes with weather conditions. This project builds regression models to predict inverter AC power from ambient temperature, module temperature and solar irradiation.

## Data
Public Plant 1 solar generation and weather sensor datasets (`Plant_1_Generation_Data.csv` and `Plant_1_Weather_Sensor_Data.csv`).
- Plant generation data: 68,778 records
- Weather sensor data: 3,182 readings
- Merged on timestamp (68,774 rows after the join)

## Features and Target
- Features: ambient temperature, module temperature, irradiation
- Target: AC power

## Models and Results
80/20 train-test split.

| Model | R² | MAE | RMSE |
|---|---|---|---|
| Linear Regression | 0.980 | 26.3 | 55.5 |
| Random Forest | 0.9865 | 16.4 | 45.7 |

Random Forest reduced the mean absolute error by about 38% compared to Linear Regression. Feature importance was also analyzed.

## Tools
Python, Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Jupyter Notebook

## How to Run
1. Place the two CSV files from the dataset in a folder.
2. Update the CSV file paths in the notebook to match where you saved them.
3. Run all cells.

## Author
Palak Rahangdale
