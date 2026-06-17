# Credit Card Fraud Detection using Machine Learning

## Oasis Infobyte Data Analytics Internship - Level 2 Project

### Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Fraud detection plays a crucial role in the financial industry by identifying suspicious transactions and preventing financial losses.

The objective of this project is to build and evaluate machine learning models capable of distinguishing between legitimate and fraudulent transactions using historical transaction data.

---

## Objective

* Perform data cleaning and preprocessing.
* Conduct exploratory data analysis (EDA).
* Understand class imbalance in fraud datasets.
* Train machine learning models for fraud detection.
* Evaluate model performance using appropriate metrics.
* Compare multiple models and identify the best-performing solution.

---

## Dataset Information

The dataset contains anonymized credit card transactions with the following characteristics:

* Total Records: 284,807
* Total Features: 31
* Target Variable: Class

  * 0 = Legitimate Transaction
  * 1 = Fraudulent Transaction

After removing duplicate records:

* Remaining Records: 283,726
* Duplicate Records Removed: 1,081

Class Distribution:

* Legitimate Transactions: 99.83%
* Fraudulent Transactions: 0.17%

The dataset is highly imbalanced, making fraud detection a challenging machine learning problem.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Project Workflow

### Data Cleaning

* Checked for missing values.
* Removed duplicate records.
* Verified dataset integrity.

### Exploratory Data Analysis

* Class distribution analysis.
* Transaction amount distribution.
* Fraud vs Non-Fraud comparison.
* Correlation analysis.

### Data Preprocessing

* Standardized Time and Amount features.
* Split data into training and testing sets.

### Model Building

The following machine learning models were implemented:

1. Logistic Regression
2. Random Forest Classifier

### Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

---

## Model Performance

### Logistic Regression

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 99.91% |
| Precision | 84.85% |
| Recall    | 58.95% |
| F1 Score  | 69.57% |
| ROC-AUC   | 79.46% |

### Random Forest Classifier

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 99.95% |
| Precision | 97.18% |
| Recall    | 72.63% |
| F1 Score  | 83.13% |
| ROC-AUC   | 86.31% |

---

## Results

The Random Forest Classifier demonstrated superior performance compared to Logistic Regression.

Key Findings:

* Achieved very high precision with minimal false positives.
* Improved recall, enabling the detection of more fraudulent transactions.
* Delivered the highest F1 Score and ROC-AUC score.
* Successfully handled a highly imbalanced dataset.

---

## Feature Importance

Feature importance analysis was performed using the Random Forest model to identify the most influential variables contributing to fraud detection.

Visualizations were created to better understand model behavior and feature contributions.

---

## Conclusion

This project successfully developed a machine learning-based fraud detection system capable of identifying fraudulent credit card transactions with high accuracy and reliability.

Among the evaluated models, Random Forest achieved the best results:

* Accuracy: 99.95%
* Precision: 97.18%
* Recall: 72.63%
* F1 Score: 83.13%
* ROC-AUC Score: 86.31%

The project demonstrates the effectiveness of machine learning techniques in detecting fraudulent activities and highlights the importance of using Recall, Precision, and F1 Score when working with highly imbalanced datasets.

---

## Future Scope

* Apply SMOTE for class balancing.
* Perform hyperparameter tuning.
* Experiment with XGBoost and LightGBM.
* Deploy the model using Flask or FastAPI.
* Build a real-time fraud detection dashboard.

---

## Internship Information

Organization: Oasis Infobyte
Domain: Data Analytics
Project Level: Level 2

---

## Author

Kushagra Pandey

B.Tech Computer Science & Engineering
Jaypee Institute of Information Technology (JIIT), Noida
