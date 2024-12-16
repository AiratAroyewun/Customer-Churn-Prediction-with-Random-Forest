# Customer-Churn-Prediction-with-Random-Forest
This project involves building a Random Forest Classifier to predict whether a customer will churn based on historical customer data. The goal was to understand the key drivers of customer churn and evaluate whether price sensitivity is the most influential factor.

# Project Outline:
* Business Problem: Investigate if price sensitivity is the most important factor driving customer churn.
* Dataset: The dataset includes features like customer demographic information, pricing data across different time ranges (peak, mid-peak, off-peak), and historical usage metrics.
* Modeling: A Random Forest model was implemented to predict churn, with hyperparameters optimized to improve the model’s performance.

# Steps:
## Exploratory Data Analysis (EDA):
* Imported the dataset and explored its structure, identified outliers, and handled them.
* Cleaned data, handled missing values, and transformed categorical variables using one-hot encoding.
## Feature Engineering:
* Log-transformed highly skewed features.
* Dropped date columns after extracting month features.
* Checked and handled multicollinearity between features.
## Modeling:
* I split the data vertically and horizontally. I created an Undersample and Oversample of the data.
* I created a Baseline for the model.
* Used Random Forest Classifier and evaluated the model with accuracy, precision, and confusion matrix metrics.
## Evaluation:
* Evaluated the model’s performance and created a visualization that displayed the feature importance to understand which factors influenced the churn prediction.
* I saved my model to a pickle file.
* Created a function that will:
    1.  Recieve a csv file path and model path
    2. Create a prediction 
    3. Add prediction and prediction probability to the existing X_test file
    4. Save the X_test into the device as a csv_file.
## Key Insights:
* Price sensitivity was not the dominant factor in churn.
* Features like net margin, customer tenure, and forecast consumption had a much stronger influence.
* Time-related features such as the number of months active were also significant predictors.
<img width="641" alt="Exec sum" src="https://github.com/user-attachments/assets/1b39b8ed-1d6f-4d1b-bf88-e02ea55dbd43" />
