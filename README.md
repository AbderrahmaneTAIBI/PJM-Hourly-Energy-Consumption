# Hourly Energy Consumption

This repository contains code that analyzes hourly energy consumption data of 11 different zones across the United States. The data is provided in the form of parquet files that preserve the schema of the data. The code uses the LightGBM machine learning algorithm to build a model that predicts the energy consumption for each zone. The repository also includes code for hyperparameter tuning of the LightGBM model using GridSearchCV.

## Libraries used:

* pandas
* numpy
* matplotlib
* seaborn
* lightgbm
* sklearn

## Exploratory Data Analysis:

The code begins by importing the necessary libraries and loading the data from the parquet file into a pandas dataframe. The first few rows and last few rows of the data are then printed to get an idea of the structure of the data. The dataframe's describe method is also called to get a summary of the statistical information about the data.

## Model Building:

LightGBM (Light Gradient Boosting Machine) is a gradient boosting framework that is designed to be both efficient and scalable. It was developed by Microsoft and is widely used in data science and machine learning applications for various tasks, including classification, regression, and ranking.

The LightGBM algorithm is used to build a model that predicts energy consumption for each zone. The data is split into training and testing datasets. The model is trained on the training dataset and evaluated on the testing dataset using the mean squared error and mean absolute error metrics.

## Hyperparameter Tuning:

The GridSearchCV function from scikit-learn is used to perform hyperparameter tuning on the LightGBM model. This is done to find the optimal values of the model's hyperparameters that result in the best performance.

## Conclusion:

This repository provides an example of using the LightGBM algorithm to predict hourly energy consumption for different zones across the United States. The code can be used as a starting point for building similar models for other types of time-series data.
