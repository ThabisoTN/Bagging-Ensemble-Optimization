# Bagging-Classifier-Tuning

## Project Overview

This project implements and optimizes a **Bagging Classifier** ensemble model using **Decision Trees** as base estimators. The goal is to improve classification accuracy by aggregating multiple decision trees trained on random subsets of data and tuning key hyperparameters for better performance.

---

## What This Project Does

This project focuses on building a robust classification model through the following steps:

1. **Bagging Classifier Implementation**  
   A Bagging Classifier is created using Decision Trees with balanced class weights to handle any class imbalance.

2. **Hyperparameter Tuning Using Randomized Search**  
   The `max_samples` parameter — which controls how many samples each base estimator trains on — is tuned using `RandomizedSearchCV`.  
   The search explores values from 500 to 1300 inclusive to find the optimal setting for highest accuracy.

3. **Training Final Tuned Model**  
   Using the best `max_samples` from tuning, a final Bagging model is trained on the training data.

4. **Performance Evaluation**  
   The final model’s accuracy is evaluated on the test set, with results printed in a clear, user-friendly format.

This approach demonstrates the power of ensemble methods combined with hyperparameter tuning to create highly effective classifiers.

---

## Features

- Decision Tree base estimators with balanced class weights.
- Bagging ensemble to reduce overfitting and improve stability.
- Randomized hyperparameter search for efficient tuning.
- Clear accuracy reporting on test data.
- Modular and adaptable code for similar classification tasks.

