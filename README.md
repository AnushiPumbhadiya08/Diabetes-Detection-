# Diabetes-Detection-
This project focuses on predicting diabetes using supervised machine learning techniques. Multiple classification models were developed, optimized, and evaluated to identify patterns in medical data and provide reliable predictions. Emphasis was placed on proper handling of missing values, feature scaling, and hyperparameter tuning to ensure robust and reproducible results..

## Problem Statement
The objective of this project is to build a machine learning-based classification system that can accurately predict whether a patient is diabetic or non-diabetic using clinical and physiological attributes. The project aims to apply best practices in data preprocessing, model training, and evaluation while ensuring interpretability and avoiding data leakage.

## Dataset
The dataset consists of several medical features, including:

Glucose

Blood Pressure

Insulin

BMI

Skin Thickness

Age

Outcome (target variable)

Although the dataset does not contain explicit null values, several features include 0 values, which represent missing measurements rather than valid physiological data. These values were handled appropriately during preprocessing.

## Data Preprocessing 
***1. Imputing Missing Values***

- Zero values were treated as missing data and replaced with NaN.

- Mean imputation was used to fill missing values for each feature.

***2. Train–Test Split***

- The dataset was divided into training and testing sets.
  
***3. Feature Scaling***

- Feature scaling was performed using StandardScaler.

- Scaling was applied inside sklearn Pipelines to prevent data leakage during cross-validation.

## Models Implemented
The following classification models were trained and evaluated:

- Logistic Regression

- Support Vector Machine (SVM)

- Random Forest Classifier

Each model was implemented using a Pipeline to ensure consistent preprocessing and fair comparison.

## Hyperparameter Tuning
- GridSearchCV was used for hyperparameter optimization.

- 5-fold cross-validation was applied.

- Accuracy was used as the primary evaluation metric.

## Evaluation Metrics (Results)

Model performance was evaluated using:

- Accuracy

- Confusion Matrix

- Precision, Recall, and F1-score

## Key Challenges Addressed

- Long execution time due to missing feature scaling

- Risk of data leakage during preprocessing

- Proper identification and handling of missing values

These challenges were resolved using feature scaling within Pipelines and structured model evaluation.

## Technologies Used

- Python

- NumPy

- Pandas

- Matplotlib / Seaborn

- Scikit-learn

## Future Improvements

- Implement advanced models such as XGBoost and LightGBM

- Apply model explainability techniques

- Deploy the model as a web application

- Expand the dataset for improved generalization

## Conclusion

This project demonstrates an end-to-end machine learning pipeline for diabetes prediction, highlighting the importance of proper preprocessing, leakage-free training, and systematic evaluation. The approach ensures reliable and interpretable results suitable for academic and real-world healthcare applications.


