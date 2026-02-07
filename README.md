Restaurant Data Analysis and Predictive Modeling
This project consists of two distinct tasks focused on analyzing a restaurant dataset to predict aggregate ratings and classify cuisines using various machine learning techniques.

Project Overview
The project is divided into two primary tasks:

Task 1: Restaurant Rating Prediction – Developing a regression model to predict the "Aggregate rating" of restaurants.

Task 3: Cuisine Classification – Developing a classification model to identify the primary cuisine of a restaurant based on its features.

Files
internship task 1 (2).ipynb: Notebook containing data preprocessing, feature engineering, and regression modeling for rating prediction.

internship task3 (2).ipynb: Notebook containing data cleaning, label encoding, and classification modeling for cuisine prediction.

Task 1: Restaurant Rating Prediction
Objectives
Build a model to predict the aggregate rating of a restaurant based on available features.

Identify the most influential features affecting restaurant ratings.

Implementation Details
Data Preprocessing:

Cleaned column names by stripping whitespace.

Handled missing values by filling numeric columns with the mean and categorical columns with "Unknown".

Converted categorical features into numerical format using one-hot encoding (pd.get_dummies).

Models Used:

Linear Regression: Achieved an R² Score of ~0.96 and an RMSE of ~0.30.

Random Forest Regressor: Used for feature importance analysis.

Key Findings:

The model demonstrated high accuracy in predicting ratings.

Top influential features include specific addresses and rating text categories like "Not rated" (negative impact) or "Excellent" (positive impact).

Task 3: Cuisine Classification
Objectives
Predict the "Primary Cuisine" of a restaurant using classification algorithms.

Evaluate model performance across different cuisine categories.

Implementation Details
Data Preprocessing:

Dropped irrelevant columns such as 'Restaurant ID', 'Address', and 'Latitude/Longitude'.

Simplified the 'Cuisines' column by extracting the first listed cuisine as the "Primary Cuisine".

Encoded the target variable using LabelEncoder and categorical features using one-hot encoding.

Models Used:

Random Forest Classifier: Trained to categorize restaurants into their respective primary cuisines.

Evaluation:

Performance was measured using a classification report and a confusion matrix.

The analysis specifically visualized the confusion matrix for the top 10 most frequent cuisines to check for misclassifications.

Requirements
To run these notebooks, the following Python libraries are required:

pandas

numpy

scikit-learn

seaborn

matplotlib

Usage
Ensure the dataset file (e.g., Dataset .csv) is placed in the correct directory path specified in the notebooks.

Run the cells sequentially to perform data cleaning, training, and evaluation.
