# App-Rating-Prediction---Python

Project Title: App Rating Prediction
This project focuses on predicting user ratings for mobile applications available on the Google Play Store. The goal is to analyze app-related data and build a machine learning model to predict app ratings more accurately.

Key Components:
1. Data Loading and Exploration
The dataset used contains information about various mobile apps. It includes fields such as app name, category, rating, number of reviews, size, installs, type, price, content rating, genres, and update dates.
Initial steps include:

Reading the dataset using pandas

Checking the structure and basic statistics

Identifying missing values

2. Data Cleaning and Preprocessing
The data required several cleaning steps before modeling:

Missing ratings were removed

App sizes were converted into consistent numerical values

The ‘Installs’ and ‘Price’ fields were cleaned to remove characters like plus signs, commas, and dollar symbols

Categorical features like ‘Type’, ‘Content Rating’, and ‘Genres’ were encoded using label encoding

Date fields were converted into datetime format and new time-based features were extracted

3. Feature Engineering
New features were created from the existing data:

Converted size values into kilobytes

Transformed ‘Last Updated’ into numeric form showing the number of days since last update

Removed outliers and performed normalization on numerical features

4. Model Building and Evaluation
Different machine learning models were tested to predict app ratings:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Models were evaluated based on performance metrics like:

Mean Absolute Error

Mean Squared Error

Root Mean Squared Error

R2 Score

Random Forest gave the best performance among the tested models.

Conclusion

The project successfully builds a predictive model using Random Forest that gives reliable estimates of app ratings based on multiple app characteristics. Proper data cleaning and feature transformation helped improve the model's accuracy.
