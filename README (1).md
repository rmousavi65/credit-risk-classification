# credit-risk-classification
Challenge_20_credit-risk-classification

# README.md

This README file provides an overview of the code and steps involved in training and evaluating a logistic regression model for loan prediction using both original and oversampled data.

## Splitting the Data

The first step involves splitting the data into training and testing sets. The lending data is read from the "lending_data.csv" file in the "Resources" folder and loaded into a Pandas DataFrame. The labels are extracted from the "loan_status" column, while the remaining columns are used as features. The balance of the labels variable is checked using the `value_counts` function. The data is then split into training and testing datasets using the `train_test_split` function.

## Logistic Regression Model with Original Data

In this section, a logistic regression model is created using the original data. The LogisticRegression module from sklearn is imported, and an instance of the model is created. The model is then fitted using the training data. Predictions are made on the testing data, and the model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

## Logistic Regression Model with Resampled Data

Here, the data is resampled using the RandomOverSampler module from the imbalanced-learn library to address class imbalance. The random oversampler model is instantiated, fitted with the original training data, and used to resample the data. The LogisticRegression model is created, fitted with the resampled training data, and used to make predictions on the testing data. The model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

## Evaluation and Comparison

The performance of both models is compared in this section. The accuracy scores, confusion matrices, and classification reports of both models are displayed. The oversampled model achieved a higher accuracy score of 99% compared to the imbalanced model's score of 95%. The oversampled model demonstrated improved performance in detecting mistakes and outliers. However, there is room for improvement in accurately identifying high-risk loans.

This README.md file provides an outline of the code and steps involved in training and evaluating the logistic regression model for loan prediction. For more details, refer to the source code file.
