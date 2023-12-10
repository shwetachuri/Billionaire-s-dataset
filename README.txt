Overview:
This Python script aims to predict whether an individual is a self-made billionaire based on various features. It utilizes pandas for data manipulation, sklearn for machine learning tasks, and a Random Forest Classifier for the prediction model.

Version:
Python 3 (ipykernal)

Dependencies:
pandas
scikit-learn

Dataset:
The dataset used is a CSV file named "BIA 500 - CAPSTONE PROJECT DATA SET (WORKING COPY).csv", which includes various attributes of billionaires. This dataset originated from the 'Billionares Statistics Dataset' from the kaggle website: https://www.kaggle.com/datasets/nelgiriyewithana/billionaires-statistics-dataset

Features:
Handling Missing Values: Missing values in numeric columns are imputed using the median strategy.
Dropping Irrelevant Columns: Columns such as personal names, dates, and geographical coordinates are dropped.
One-Hot Encoding: Categorical variables are transformed using one-hot encoding.
Handling NaN Values Post-Encoding: Any NaN values after encoding are replaced with zero.
Target Variable
The target variable is 'selfMade', indicating whether an individual is a self-made billionaire.

Model Training and Evaluation:
Data Splitting: The dataset is split into training and testing sets (70% training, 30% testing).
Random Forest Classifier: A Random Forest model with 150 estimators with infinite depth are trained on the dataset.
Evaluation: The model's performance is evaluated using accuracy score and classification report.
Feature Importance Analysis
The script also provides an analysis of the importance of different features in the prediction.

Usage:
To run the script, ensure the path to the dataseet reflects the user's specific dataset location. 
Install the required dependencies and execute the script.

Output:
The first few rows of the dataset for inspection.
Balance of the target variable 'selfMade'.
Summary statistics of the dataset.
Accuracy of the self-made billionaire prediction.
Classification report.
Feature importances in the model.
