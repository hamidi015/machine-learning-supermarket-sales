:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
Supermarket Sales Prediction Challenge
Project Overview
In this project, I built several machine learning models to predict supermarket sales quantity (Quantity_Sold_(kilo)) using historical sales data.

Dataset
The project uses:

labeled_data.csv (training data)
unlabeled_data.csv (prediction data)
Data Preparation
Checked missing values
Handled missing values using median imputation
Encoded categorical features using One-Hot Encoding
Split the dataset into training and validation sets
Models Tested
Linear Regression
Ridge Regression
Random Forest Regression
Results
Model	MAE	MSE	R²
Linear Regression	7.650	145.875	-0.000
Ridge Regression	6.948	129.610	0.111
Random Forest	4.294	65.599	0.550
Best Model
Random Forest achieved the best performance and was selected as the final model.

Key Learnings
Feature Engineering
Missing Value Handling
One-Hot Encoding
Model Evaluation
Regression Models
Machine Learning Workflow
Technologies
Python
Pandas
Scikit-Learn
Jupyter Notebook
Git & GitHub

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::