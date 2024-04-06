# SMAI Assignment 4 README

This README provides an overview of the completed tasks for the Statistical Methods in Artificial Intelligence (SMAI) Assignment 4.

## Tasks

The tasks in Section 3 and Section 4 of the assignment were performed on both regression and classification tasks using the following datasets:
- Classification: Wine Quality Dataset
- Regression: Boston Housing Dataset

Modularized code with appropriate functions was created to make the code short and precise.

## 3. Ensemble Learning

### 3.1 Pre-Requisite
- Implemented and tuned the following types of models (List 1 models):
  - Decision Trees (using sklearn)
  - Logistic and Linear Regressor for Classification and Regression respectively
  - Multi-Layer Perceptron

### 3.2 Bagging
For both classification and regression tasks:
1. Designed a function that performs the bagging methodology of ensemble learning with the following input parameters:
   - Base Estimator Model (List 1 models)
   - Number of Estimators (variable according to the base-estimator)
   - Fraction/Number of Samples (0.15, 0.25, 0.5, 0.75, 1.0)
   - Bootstrap (True: Sampling with replacement, False: Sampling without replacement)
   - Voting Mechanism (Hard Voting, Soft Voting)
2. Trained ensemble models across all combinations of parameters and reported the best-performing models
3. Plotted a heatmap for the accuracies obtained by each class of base estimator models across Fraction of Samples and Number of Estimators
4. Compared the performance of each model in List 1 models with the best-performing ensemble model of the same class using a single side-by-side histogram

### 3.3 Stacking
1. Designed a function that performs the stacking methodology of ensemble learning with the following input parameters:
   - Level-0 estimators (List 1 Models)
   - Level-1 estimators (Logistic and Linear Regressor for classification and regression, Decision Tree)
   - Stacking Methodologies (Stacking, Blending)
2. Trained ensemble models across all combinations of parameters and reported the best-performing models
3. Compared the accuracies and training time of the best-performing models of Bagging and Stacking ensembles for each Base Estimator Model class

## 4. Random Forest vs Boosted Trees

1. Trained a Random Forest Classifier and Regressor and reported the best-performing hyperparameters
2. Compared the results of the best Random Forest with the following Boosted Decision Trees:
   - Decision Trees + AdaBoost
   - Gradient Boosted Decision Trees
   - Experimented with the number of estimators and plotted their training times and accuracies
3. Provided an analysis of the mistakes of these models and explored and explained the feature similarity of the common mistakes

The code for this assignment can be found in the Jupyter Notebook file.
