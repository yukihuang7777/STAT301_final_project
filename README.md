# Spam Email Prediction

## Author: Jake Andersen-Lum, Stephen Hong, Yicheng Huang, Ella Ren

## Project Summary
This project investigates the use of logistic regression with LASSO regularization to classify emails as spam or non-spam. The aim is to effectively identify the most predictive variables for classifying spam emails and develop an interpretable model with strong predictive performance.

The dataset is called [email](https://www.openintro.org/data/index.php?data=email), which is sourced from OpenIntro, and the source is the first three months of 2012 for David Diez's Gmail Account.

## Project Objectives

- Perform data cleaning amd exploratory data analysis.

- Apply logistic regression with LASSO for variable selection.

- Construct a predictive model classifying emails as spam or non-spam.

- Evaluate model performance using ROC curves and confusion matrices.

## Methodology

- Irrelevant and low-variance predictors is removed to simplify the dataset.

- Dataset is randomly divided into training (70%) and test sets (30%).

- Logistic regression with LASSO is utilized for automatic feature selection.

- Model performance is validated using 5-fold cross-validation on our training data, optimizing for AUC.

- Model is improved by adjusting the classification threshold based on ROC curve.

## Conclusions

Logistic regression with LASSO regularization successfully identified critical predictors for spam emails, providing a predictive model with high interpretability. By adjusting the classification threshold based on ROC curve analysis, the model achieved much higher sensitivity, making it more suitable for real-world spam detection where false negatives are costly.

## Dependencies

The project was executed in R, using:

- `caret`

- `glmnet`

- `pROC`

- `tidyverse`