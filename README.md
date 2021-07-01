
# Credit Risk Analysis

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/Credit_Cards.png"></br>

## Overview of the Loan Prediction Risk Analysis

A common problem in assessing credit risk is the inherent imbalance (unequal 
distribution of data) between "good" risk and "bad" risk. The overwhelming 
majority will be "good" risk, and a small minority "bad". This imbalance means 
that we need to train resampling models to account for the imbalance in order 
to provide reliable results.

## Results:

In this analysis we addressed data imbalance via the following six resampling models 

- **Model 1: Naive Random Oversampling</br>**
In this model we randomly duplicate examples in the minority class to improve balance.

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/naive_random_oversampling.png"></br>

- **Model 2: SMOTE Oversampling</br>**
In this model we use the Synthetic Minority Over-sampling Technique (SMOTE) 
to balance the class distribution by randomly increasing (by replicating them)
the minority class examples.

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/SMOTE_oversampling.png"></br>

- **Model 3: Undersampling</br>**
In this model we remove examples from the training dataset of the majority class.

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/undersampling.png"></br>

- **Model 4: Combination (Over and Under) Sampling</br>**
In this model we use the SMOTEENN approach to resampling. This combines the
oversampling of SMOTE and clean the resulting data by undersampling via ENN 
(Edited Nearest Neighbors).

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/combination.png"></br>

- **Model 5: Balanced Random Forest Classifier</br>**
This model combines data trees into a forest of trees to create a final prediction
based on the accumulation of the trees in the forest.

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/balanced_random_forest.png"></br>

- **Model 6: Easy Ensemble AdaBoost Classifier</br>**
In ensemble learning we combine multiple models both to improve the accuracy of the 
model and to decrease the its variance.

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/easy_ensemble_AdaBoost_classifier.png"></br>

## Summary:

The purpose of this analysis was to determine which of the models was most reliable in detecting high risk loans ("bad" risk). 
The first question to answer is whether precision or sensitivity is most important. For this analysis I concluded that precision
is more important than sensitivity. I believe it is more important to identify "bad" risk and possibly allow a small
number of "bad" risk credit to be extended than to deny credit to a "good" risk candidate. There are options available for
companies to address repayment problems in order to mitigate loss, while companies face the prospect of absolute loss of revenue 
if they decline "good" risk candidates.

The best performing models in assessing precision are:


There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)

<img src="https://github.com/tn64/Credit_Risk_Analysis/blob/main/Resources/last_cc.png">
<!-- Photo by Dom J from Pexels -->


