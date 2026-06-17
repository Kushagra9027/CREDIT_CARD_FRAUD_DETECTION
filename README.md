# Credit Card Fraud Detection using Machine Learning

## Oasis Infobyte Data Analytics Internship - Level 2 Project

### Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Fraud detection plays a crucial role in the financial industry by identifying suspicious transactions and preventing financial losses.

The objective of this project is to build and evaluate machine learning models capable of distinguishing between legitimate and fraudulent transactions using historical transaction data.

> **Note:** The dataset is not included in this repository due to GitHub file size limitations. Please download it from the Kaggle link provided below.

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
* Target Variable: `Class`

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

## Dataset

The dataset used in this project is publicly available on Kaggle.

**Dataset Link:**
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Due to GitHub file size limitations, the dataset is not included in this repository. Please download the dataset and place the `creditcard.csv` file in the project directory before running the notebook.

### Dataset Features

* **Time** – Time elapsed between transactions.
* **V1 – V28** – PCA-transformed anonymized features.
* **Amount** – Transaction amount.
* **Class**

  * 0 = Legitimate Transaction
  * 1 = Fraudulent Transaction

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Cleaning

* Checked for missing values.
* Removed duplicate records.
* Verified dataset quality and consistency.

### 2. Exploratory Data Analysis (EDA)

* Analyzed class distribution.
* Visualized transaction amount distributions.
* Compared fraudulent and non-fraudulent transactions.
* Performed correlation analysis.

### 3. Data Preprocessing

* Standardized `Time` and `Amount` features.
* Split the dataset into training and testing sets.

### 4. Model Building

The following machine learning models were implemented:

#### Logistic Regression

Used as a baseline classification model for fraud detection.

#### Random Forest Classifier

Used an ensemble learning approach to improve prediction performance and fraud detection capability.

### 5. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score

---

## Exploratory Data Analysis

Key insights obtained during EDA:

* No missing values were found in the dataset.
* 1,081 duplicate records were identified and removed.
* The dataset is highly imbalanced, with fraudulent transactions accounting for only 0.17% of all transactions.
* Transaction amounts exhibit a heavily right-skewed distribution.
* Several anonymized features showed strong relationships with fraudulent activity.

---

## Model Performance

### Logistic Regression

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 99.91% |
| Precision | 84.85% |
| Recall    | 58.95% |
| F1 Score  | 69.57% |
| ROC-AUC   | 79.46% |

### Random Forest Classifier

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 99.95% |
| Precision | 97.18% |
| Recall    | 72.63% |
| F1 Score  | 83.13% |
| ROC-AUC   | 86.31% |

---

## Results

The Random Forest Classifier outperformed Logistic Regression across all evaluation metrics.

### Key Findings

* Achieved excellent classification performance.
* Significantly improved fraud detection recall.
* Reduced false positive predictions.
* Delivered the highest F1 Score and ROC-AUC Score.
* Demonstrated strong effectiveness on a highly imbalanced dataset.

---

## Feature Importance Analysis

Feature importance analysis was performed using the Random Forest model to identify the most influential variables contributing to fraud detection.

The top features were visualized using a feature importance chart, providing insights into which transaction characteristics were most useful for classification.

---

## Conclusion

This project successfully developed a machine learning-based fraud detection system capable of identifying fraudulent credit card transactions with high accuracy and reliability.

Among the evaluated models, Random Forest achieved the best performance:

* Accuracy: 99.95%
* Precision: 97.18%
* Recall: 72.63%
* F1 Score: 83.13%
* ROC-AUC Score: 86.31%

The results demonstrate the effectiveness of ensemble learning techniques for fraud detection. Due to the highly imbalanced nature of the dataset, evaluation metrics such as Precision, Recall, F1 Score, and ROC-AUC were prioritized over accuracy alone.

---

## Future Improvements

* Apply SMOTE for class balancing.
* Perform hyperparameter tuning.
* Experiment with XGBoost and LightGBM.
* Deploy the model using Flask or FastAPI.
* Build a real-time fraud monitoring dashboard.
* Implement anomaly detection techniques.

---

## Repository Structure

```text
Fraud-Detection/
│
├── notebooks/
│   └── Fraud_Detection.ipynb
│
├── images/
│   ├── class_distribution.png
│   ├── confusion_matrix.png
│   └── feature_importance.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Internship Information

Organization: Oasis Infobyte
Domain: Data Analytics
Project Level: Level 2

---

## Author

**Kushagra Pandey**

B.Tech Computer Science & Engineering
Jaypee Institute of Information Technology (JIIT), Noida

### Connect With Me

* GitHub: https://github.com/Kushagra9027
* LinkedIn: Add your LinkedIn profile link here
