# Parkinson's Disease Prediction - Ensemble Classification
**Course:** _DA5030 - Introduction to Machine Learning & Data Mining_

## Overview
This project builds an ensemble classification model to predict whether a patient has Parkinson's Disease. The ensemble combines decision tree based methods (**random forest**) with **logistic regression** models to improve accuracy and robustness.

## Data
The following data was provided and was loaded using their URLs:
* **Training Data:** [parkinsons-diagnostic-data.csv](https://s3.us-east-2.amazonaws.com/artificium.us/datasets/parkinsons-diagnostic-data.csv)
* **Validation Data:** [parkinsons-diagnostic-validation-100.csv](https://s3.us-east-2.amazonaws.com/artificium.us/datasets/parkinsons-diagnostic-validation-100.csv)

## Deliverables
* `Parkinson_Classification.Rmd` - R Notebook
* `Parkinson_Classification.html` - knitted HTML report
* `Parkinsons.Predictions.csv` - predictions for the validation set

## Tools & Skills
### Languages & Environment: 
* R
* RStudio

### Dependencies:
This project uses the following packages:
* dplyr
* ggplot2
* kableExtra
* knitr
* caret
* randomForest

## Methodology
1. Load Data
2. Explore Data
3. Shape Data
   * Remove missing data and identifiers
   * Perform transformations for Random Forest model
   * Perform transformations for Logistic Regression model
   * Handle outliers
   * Visualize and handle distribution
   * Encode categorical variables
   * Multicollinearity
4. Random Forest Model
   * Train
   * Evaluate
5. Homogeneous Logistic Regression Model
   * Train
   * Evaluate
6. Build Heterogeneous Ensemble Model
7. Evaluate and Tune Ensemble Model
8. Model Validation
   * Load validation set
   * Prepare validation set
   * Predict validation set

## Results
The final predictions were saved in the  `Parkinsons.Predictions.csv` file which consists of the _PatientID_ and _Diagnosis_. The models are evaluated using Overall Accuracy, True Positive Rate, True Negative Rate, Precision, and F1-score. The full analysis and report could be found [here](https://zoechow24.github.io/parkinsons-classification-ensemble/Parkinson_Classification.html). 


   
