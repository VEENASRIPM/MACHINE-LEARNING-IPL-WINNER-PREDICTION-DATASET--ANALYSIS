-- Objective
This project aims to investigate the effectiveness of various supervised learning models in forecasting IPL match outcomes based on categorical pre-match features, with the goal of identifying the most accurate and generalizable approach.

-- Key Processes

  -- Data Preprocessing
Handling null values and duplicates.
Encoding categorical variables using LabelEncoder/OneHotEncoder.
Train-test split (typically 70-30 or 80-20).
Feature scaling using StandardScaler where required.

   ---Model Development
Implemented algorithms:

-Logistic Regression
-K-Nearest Neighbors (KNN)
-Support Vector Machine (SVM)
-Decision Tree
-Random Forest
-Nive bayes

-- Performance measured using accuracy, confusion matrix, and classification report.

  ---Class Imbalance Handling
SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset.
Applied only to the training data after the split.

   ---Feature Importance & Reduction
The 'venue' feature was identified as potentially leading to overfitting due to its strong correlation with outcomes.
Models were re-trained after removing 'venue' to check for generalization improvement.
Performance comparison before and after removal shows improved model robustness and reduced overfitting.

-- Results Summary

Accuracy
Without SMOTE	Moderate	Class imbalance affected minority class
With SMOTE	Improved	Balanced class distribution helped accuracy
Venue Feature Retained	High	Risk of overfitting observed
Venue Feature Removed	Stable	Better generalization, less overfitting

-- Conclusion
SMOTE effectively improved prediction on minority classes.
Removing 'venue' reduced overfitting and led to more reliable accuracy across splits.
Feature selection and data balancing are crucial steps for model generalization.

-- Reported by
