# Heart Disease Prediction

This project aims to predict the risk of heart disease in patients using a variety of machine learning models. The dataset includes several features related to health and lifestyle, and the target variable is whether a patient develops heart disease over ten years.

## Dataset

The dataset contains the following columns:
- `male`: Gender of the patient (1 = Male, 0 = Female)
- `age`: Age of the patient
- `currentSmoker`: Whether the patient is a current smoker (1 = Yes, 0 = No)
- `cigsPerDay`: Number of cigarettes smoked per day
- `BPMeds`: Whether the patient is on blood pressure medication (1 = Yes, 0 = No)
- `prevalentStroke`: History of stroke (1 = Yes, 0 = No)
- `prevalentHyp`: History of hypertension (1 = Yes, 0 = No)
- `diabetes`: Whether the patient has diabetes (1 = Yes, 0 = No)
- `totChol`: Total cholesterol level
- `sysBP`: Systolic blood pressure
- `diaBP`: Diastolic blood pressure
- `BMI`: Body Mass Index
- `heartRate`: Heart rate
- `glucose`: Glucose level
- `TenYearCHD`: Whether the patient developed heart disease over ten years (1 = Yes, 0 = No)

## Data Preprocessing

1. **Handling Missing Values**:
   - Dropped the `education` column due to a significant number of missing values.
   - Filled missing values in categorical columns with the mode.
   - Filled missing values in continuous columns with the median.

2. **Resampling**:
   - The dataset was imbalanced, so resampling was performed to balance the classes.

## Model Selection

Various machine learning models were trained and evaluated:

- **Random Forest Classifier**
- **AdaBoost Classifier**
- **Gradient Boosting Classifier**
- **Logistic Regression**
- **Support Vector Classifier (SVC)**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Gaussian Naive Bayes**
- **XGBoost Classifier**

### Evaluation Metrics

Each model was evaluated using the following metrics:
- Accuracy
- Classification Report (Precision, Recall, F1-Score)
- Confusion Matrix

### Best Model

The Random Forest Classifier achieved the highest accuracy of 97.36% and demonstrated robust performance across all evaluation metrics.

## Predictive System

A predictive system was developed to classify whether a new patient has a risk of developing heart disease based on their health parameters. This system uses the trained Random Forest model.

### Usage

To use the predictive system, provide the following patient information:
- Gender
- Age
- Smoking status
- Number of cigarettes per day
- Blood pressure medication status
- Stroke history
- Hypertension history
- Diabetes status
- Total cholesterol level
- Systolic blood pressure
- Diastolic blood pressure
- Body Mass Index (BMI)
- Heart rate
- Glucose level

The system will output whether the patient is at risk of heart disease.

## Conclusion

This project successfully demonstrates the use of machine learning for predicting heart disease risk. The Random Forest Classifier, in particular, proved to be highly effective in this task. This model can potentially assist healthcare professionals in early diagnosis and intervention for patients at risk of heart disease.
