# Industrial-Copper-Modeling

# Copper Industrial Dataset Analysis and Prediction
This repository contains code for data cleaning, analysis, and prediction using the Copper Industrial Dataset. The dataset includes information on various copper products, their quantities, and related selling prices. The analysis includes data preprocessing, outlier handling, feature transformation, and machine learning modeling for regression and classification tasks.

Table of Contents,
Project Overview,
Requirements,
Data Cleaning and Preprocessing,
Exploratory Data Analysis,
Machine Learning Models,
Decision Tree Regressor,
Decision Tree Classifier,
Usage.

# Project Overview:
The goal of this project is to:

Clean and preprocess the Copper Industrial Dataset.
Perform exploratory data analysis to understand data distributions and correlations.
Build and evaluate machine learning models for predicting selling prices and the status of orders.
Save the trained models for future predictions.
# Requirements:
To run the code in this repository, you need to have the following packages installed:

pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
warnings
pickle

# Data Cleaning and Preprocessing:
The data cleaning steps include:

Reading the dataset from a CSV file.
Converting date columns to datetime format.
Handling null values in various columns.
Removing invalid entries (e.g., negative or zero values in quantity and thickness).
Applying log transformation to normalize skewed data.
python


# Exploratory Data Analysis
Exploratory data analysis involves visualizing the distributions and correlations in the dataset.




Usage
To use the code in this repository, follow these steps:

Clone the repository to your local machine.
Ensure all required packages are installed.
Run the provided Python scripts for data cleaning, analysis, and modeling.
Use the trained models to make predictions on new data samples.
Save and load the models using pickle for future use.
