# Module 20 Report

## Overview of the Analysis

This project focuses on using the Logistic Regression model to analyze a historic lending dataset. The main objectives of the analysis are as follows:

1. To train a Logistic Regression model to assess the creditworthiness of borrowers based on their financial information.
2. The dataset contains loan_size and other financial variables of loan applicants, with the model learning to predict the loan_status based on this information.
3. The loan_status variable has two values: 0 and 1, representing low-risk and high-risk lending respectively.
4. The machine learning process applied to the dataset includes:
   - Supervised learning using labeled data (X and y).
   - Splitting the data into train and test sets.
   - Building a model with appropriate features.
   - Training the model using the train set and making predictions on new data.
   - Evaluating the model's performance using accuracy metrics.
   - Creating a confusion matrix and generating a report based on the analysis.

5. Logistic Regression is a binary classification model used for supervised machine learning. It categorizes data into two groups based on their properties.

## Results

The analysis includes two machine learning models:

1. Machine Learning Model 1: Logistic Regression

   - Model accuracy: 99%
   - Precision for high-risk loans: 87%; low-risk loans: 100%
   - Recall scores for high-risk loans: 89%; low-risk loans: 100%

2. Machine Learning Model 2: Logistic Regression with Random Oversampling

   - Model accuracy: 100%
   - Precision for high-risk loans: 87%; low-risk loans: 100%
   - Recall scores for high-risk loans: 100%; low-risk loans: 100%

## Summary

The Logistic Regression models used in this analysis performed well, but there is room for improvement. To achieve more accurate predictions, alternative models such as Support Vector Machines (SVM) and Random Forest could be considered.

The Logistic Regression model with Random Oversampling showed higher efficiency in predicting high-risk loans due to balanced datasets with an equal distribution of y labels (0 and 1).

Both models demonstrated different prediction rates for high-risk and low-risk loans. Considering the business context, where minimizing risk is crucial, the accuracy of low-risk loan predictions (100%) is of utmost importance.

However, it is important to note that these models may not be reliable in classifying data points that fall near the boundary between low and high-risk loans. In such cases, SVM algorithms can be more powerful as they can more clearly differentiate and classify different data points.

Overall, I do not recommend relying solely on the above models. Exploring alternative algorithms, particularly SVM, would likely yield more robust predictions in this lending analysis.