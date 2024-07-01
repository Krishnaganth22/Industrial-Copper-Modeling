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

# Streamlit app :
Streamlit application for predicting the selling price and status of industrial copper products. The application uses machine learning models to make predictions based on various features such as quantity, thickness, width, customer ID, and more.

Installation
Clone the repository:

sh
Copy code
git clone https://github.com/yourusername/industrial-copper-modeling.git
cd industrial-copper-modeling
Create a virtual environment and activate it:

sh
Copy code
python -m venv venv
source venv/bin/activate # On Windows use `venv\Scripts\activate`
Install the required dependencies:

sh
Copy code
pip install -r requirements.txt
Usage
To run the Streamlit application, use the following command:

sh
Copy code
streamlit run app.py
This will start the Streamlit server and open the application in your default web browser.

Data Preprocessing
The data preprocessing includes the following steps:

Loading the Data: The data is loaded from a CSV file.
Date Conversion: The Item_date and Delivery_date columns are converted to datetime format.
Handling Missing Values:
Missing values in the Material_ref column are filled with 'Unknown'.
Rows with other missing values are dropped.
Data Cleaning: Negative or zero values in Selling_price, Quantity_tons, and Thickness are handled.
Log Transformation: Log transformation is applied to Selling_price, Quantity_tons, and Thickness to normalize the data.
Model Training
Selling Price Prediction
Features: Quantity_tons_log, Status, Item_type, Customer, Country, Application, Product_ref, Width, Thickness_log
Target: Selling_log
Encoding: One-hot encoding for Item_type and Status.
Scaling: Standard scaling for numerical features.
Model: Decision Tree Regressor with hyperparameter tuning using GridSearchCV.
Status Prediction
Features: Quantity_tons_log, Selling_log, Item_type, Application, Thickness_log, Width, Country, Customer, Product_ref
Target: Status
Encoding: One-hot encoding for Item_type.
Scaling: Standard scaling for numerical features.
Model: Decision Tree Classifier.
Streamlit Application
The Streamlit application provides two tabs for predicting the selling price and status of copper products.

Tab 1: Predict Selling Price
Inputs: Status, Item Type, Country, Application, Product Reference, Quantity Tons, Thickness, Width, Customer ID.
Output: Predicted Selling Price.
Tab 2: Predict Status
Inputs: Quantity Tons, Thickness, Width, Customer ID, Selling Price, Item Type, Country, Application, Product Reference.
Output: Predicted Status (Won/Lost).
Contributing
Contributions are welcome! Please create a pull request or open an issue to discuss your changes.
