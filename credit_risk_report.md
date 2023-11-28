# Module 12 Report Template

## Overview of the Analysis

The purpose of this project is to create a machine learning model that can accurately predict based on borrower data such as loan size, interest rate, borrower income and total debt, whether loaning money to the borrower would be safe or high risk. The data was split into training and testing data with the column "loan_status" reflecting whether a loan was risky or not, through the use of a logistic regression model, was able to accurately predict the correct loan status at a 95% rate. However, our data contained 75036 instances of healthy loans and 2500 instances of high risk loans, therefore because of the disparity between the amount of healthy and high risk loans I decided to use random oversampling to handle any imbalances with having so few high risk loans, which resulted in a 99% accuracy rate.

## Results

* Machine Learning Model 1:
  * Balanced accuracy score: 0.952
  * Precision 0: 1.00
  * Precision 1: 0.85
  * Recall 0: 0.99 
  * Recall 1: 0.91


* Machine Learning Model 2:
  * Balanced accuracy score: 0.994
  * Precision 0: 1.00
  * Precision 1: 0.84
  * Recall 0: 0.99 
  * Recall 1: 0.99

## Summary

In conclusion I reccomend the second model, aka the model where random oversampling was used to balance the data, at least for when trying to predict whether a borrower's data reflects a safe loan. Compared to the first model, the second model has a lower number of false negatives, meaning that if the model predicts a loan to be safe, it almost always will be safe. This is also the most important factor for the loaner, because it is more important for them to know if a loan is guarenteed safe, rather than knowing if a loan is guarenteed unsafe.