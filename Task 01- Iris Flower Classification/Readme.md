### Iris Flower Classification

## Overview
This task, completed for a CodeAlpha internship, involves classifying Iris flower species (setosa, versicolor, virginica) using the Iris.csv dataset. The goal was to preprocess data, visualize features, and train classification models.

## Dataset

File: Iris.csv
Columns: Id, SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm, Species
Size: 150 rows
Features: SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm
Target: Species (categorical)
Issues: No missing values; fixed a visualization error.

## Methodology

Data Cleaning:
Dropped Id column.
Correctly selected features excluding Species and Id.


## Exploration:
Checked data types and class distribution (~50 samples per species).


## Visualization:
Used pairplots and boxplots to show feature distributions.
Fixed boxplot issue for proper display.


## Preprocessing:
Encoded Species with LabelEncoder.
Scaled features with StandardScaler.
Split data (80% train, 20% test).


## Modeling:
Trained Logistic Regression and Decision Tree models.
Evaluated with accuracy and confusion matrix.


## Tools: Pandas, Scikit-learn, Matplotlib, Seaborn

## Results

Accuracy: ~93% (Logistic Regression), ~90% (Decision Tree).
Key Finding: Petal features (PetalLengthCm, PetalWidthCm) were most important.
Visualization: Boxplots showed clear separation for setosa.

## Insights

Application: Useful for plant identification in agriculture or botany.
Improvement: Could use ensemble models like Random Forest.
Code: irisFlowerClassification.ipynb
