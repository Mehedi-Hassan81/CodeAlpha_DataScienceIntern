### Sales Prediction

## Overview
This task, completed for a CodeAlpha internship, predicts sales based on advertising spend using the Advertising.csv dataset. The goal was to preprocess data, train a regression model, analyze advertising impact, and provide marketing insights.
Dataset

## File: Advertising.csv
Columns: Unnamed: 0, TV, Radio, Newspaper, Sales
Size: 200 rows
Features: TV, Radio, Newspaper (advertising spend)
Target: Sales
Issues: No missing values; dropped Unnamed: 0.

## Methodology

## Data Cleaning:
Dropped Unnamed: 0 (index).
Checked for outliers (retained for simplicity).


## Preprocessing:
Selected TV, Radio, Newspaper as features.
Scaled features with StandardScaler.
Split data (80% train, 20% test).


## Modeling:
Trained Linear Regression model.
Evaluated with Mean Absolute Error (MAE) and R² score.


## Analysis:
Analyzed feature coefficients for advertising impact.
Visualized actual vs. predicted sales and sales vs. spend.


## Tools: Pandas, Scikit-learn, Matplotlib

## Results

## Performance: MAE ~1.25, R² ~0.90.
Key Finding: TV advertising had the strongest impact.
Visualization: Scatter plots confirmed TV’s high correlation with sales.

## Insights

Application: Optimizes marketing budgets for retail or e-commerce.
Recommendations: Prioritize TV advertising; test targeted campaigns.
Code: salesPrediction.ipynb
