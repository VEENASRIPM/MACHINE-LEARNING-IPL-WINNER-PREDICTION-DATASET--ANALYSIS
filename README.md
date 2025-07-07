 IPL WINNER PREDICTION USING  MACHINE LEARNING

---

 Objective

To explore multiple machine learning models and preprocessing techniques for predicting IPL match outcomes. The goal is to identify which algorithm, paired with appropriate sampling and feature engineering methods, delivers the best performance.

---

 Key Processes

-- Data Preprocessing

Handling null values and removing duplicate records.

Encoding categorical variables using LabelEncoder and OneHotEncoder.

Splitting the data into training and testing sets (70-30 or 80-20 ratio).

Applying feature scaling using StandardScaler where needed.

-- Model Development

The following algorithms were implemented and evaluated:

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Decision Tree

Random Forest

Naive Bayes

-- Performance Metrics used:

Accuracy Score

Confusion Matrix

Classification Report

-- Class Imbalance Handling

Used SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

Applied only to the training set post split to avoid data leakage.

Significantly improved the model's ability to predict minority classes.

-- Feature Importance & Reduction

The 'venue' feature was identified as highly correlated with the target.

Its inclusion caused overfitting, as it leaked outcome-related information.

Models were retrained after removing 'venue', resulting in better generalization and improved robustness.

---

-- Conclusion

SMOTE significantly enhanced prediction for underrepresented classes.

Removing the 'venue' feature helped reduce overfitting and improved model generalization.

A combination of feature selection, class balancing, and appropriate model choice is key to robust performance.

---

## PRESENTED BY

**VEENA SRI P M**  

*Data Analytics and Data Science*


---
