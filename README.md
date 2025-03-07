 # Credit Risk Analysis Report

## Overview of the Analysis

The purpose of this analysis was to evaluate the creditworthiness of borrowers using historical lending data from a peer-to-peer lending services company. The dataset contains financial information on loans, and the goal is to predict whether a loan is healthy (0) or high-risk (1). The analysis involved the following key stages:

- **Data Preparation:**  
  The dataset was first separated into features (X) and labels (y), with `loan_status` serving as the target variable.
  
- **Data Splitting:**  
  The data was split into training and testing sets using `train_test_split` with a specified `random_state` for reproducibility.
  
- **Model Training:**  
  A logistic regression model was implemented and trained using the training data.
  
- **Model Evaluation:**  
  The model’s performance was evaluated using a confusion matrix and a classification report to derive key metrics such as accuracy, precision, and recall.

## Results

The performance of the logistic regression model was summarized by the following metrics:

* **Machine Learning Model 1: Logistic Regression**
    * **Accuracy:** 0.99 
    * **Precision:** 0.99
    * **Recall:** 0.99

## Summary

The logistic regression model shows robust performance in identifying healthy loans (0) with high accuracy and precision. However, the recall for high-risk loans (1) is comparatively lower, which suggests that the model may be missing some high-risk cases. This trade-off is important in credit risk management; while it minimizes false positives, there is a potential risk if high-risk loans are not fully captured.

**Recommendation:**  
Based on the analysis, the logistic regression model is a strong baseline for credit risk classification. It is recommended for initial screening due to its overall performance and simplicity. Nonetheless, if identifying high-risk loans is critical, further improvements—such as threshold tuning, additional feature engineering, or exploring more complex models—may be necessary to enhance recall. Overall, the model is suitable for use with the understanding that further refinement could lead to better risk detection.
