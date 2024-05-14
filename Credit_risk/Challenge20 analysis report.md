# Challenge 20 Analysis Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:


This purpose of this analysis was to take in various financial datapoints and predict if a loan to the individual would be most likely to be a "healthy loan" or a "high-risk loan".  

The financial information provided was the size of the loan requested, interest rate, borrower's income, the debt to income ratio, number of accounts, whether there were any 'derogatory marks' on the borrower (such as former default, perhaps), and their total debt.  This information was used to predict if this loan would be predicted "healthy" (likely to be paid back in a timely manner), or "high-risk" (more likely to be paid back late or not at all).

To accomplish this analysis, the data provided was split into training and testing sets and scaled to make the numbers comparable.  The logistic regression model was used and once the data was trained, the test data was used to calculate the accuracy of the model.


## Results

* The precision of predicting 'healthy' loans was 1.00
* The recall of predicting 'healthy' loans was 0.99
* The precision of predicting 'high-risk' loans was 0.84
* The recall of predicting 'high-risk' loans was 0.98
* The overally accuracy was 0.99


## Summary

Overall, the logistic regression model does a good job of recall on both types of loans (meaning the model is very good at finding all of the positive predictions without returning false negatives).  However, the precision was much better for predicting 'healthy' loans (meaning the model is less likely to return a false positive from this category).  The overall accuracy of the model is pretty good, but closer attention should be paid to predictions of 'high-risk', since that has the most likelihood to produce a false positive.  Continuing to refine the model with additional training data would likely help it improve over time.  
