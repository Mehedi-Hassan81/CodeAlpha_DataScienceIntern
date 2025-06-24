### Car Price Prediction

## Overview
This task, part of a CodeAlpha internship, predicts car selling prices using the car_data.csv dataset. The goal was to preprocess data, engineer features, train a regression model, and evaluate performance.
Dataset

File: car_data.csv
Columns: Car_Name, Year, Selling_Price, Present_Price, Driven_kms, Fuel_Type, Selling_type, Transmission, Owner
Size: 301 rows
Features: Year, Present_Price, Driven_kms, Fuel_Type, Selling_type, Transmission, Owner, Car_Name (brand extracted)
Target: Selling_Price (in lakhs)
Issues: No missing values.

## Methodology

Data Cleaning:
No missing values to handle.


## Feature Engineering:
Extracted Brand from Car_Name (e.g., "Honda" from "Honda City").
Calculated Age (2025 - Year).


## Preprocessing:
One-hot encoded categorical variables (Fuel_Type, Selling_type, Transmission, Brand).
Scaled numeric features with StandardScaler.
Split data (80% train, 20% test).


## Modeling:
Trained Linear Regression model.
Evaluated with Mean Absolute Error (MAE) and R² score.


## Tools: Pandas, Scikit-learn, Matplotlib

## Results

## Performance: MAE ~1.20 lakhs, R² ~0.85.
Key Finding: Present_Price and Brand strongly influence prices.
Visualization: Scatter plot showed predicted vs. actual prices.

## Insights

Application: Helps buyers, sellers, and dealerships set fair prices.
Improvement: Could try Random Forest for better accuracy.
Code: carPricePrediction.ipynb
