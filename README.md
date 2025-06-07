---

# Breast Cancer Diagnosis using Logistic Regression

---

## Project Overview

This notebook presents a binary classification task using logistic regression to predict the malignancy of breast tumors. It follows a full machine learning pipeline, from preprocessing raw medical data to model evaluation using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

---

## Objectives

* Clean and prepare raw tumor diagnostic data.
* Train a logistic regression model to classify tumor status.
* Evaluate the model’s performance using multiple metrics.
* Interpret feature importance and diagnostic quality through ROC analysis.

---

## Methodology

### 1. Data Preprocessing

* Removed irrelevant columns such as patient identifiers.
* Re-encoded categorical diagnosis outcomes into binary form (0 = benign, 1 = malignant).
* Dropped rows with missing values to ensure data integrity.

### 2. Data Splitting

* Stratified train-test split (70% training, 30% testing).
* Preserved class distribution across splits to maintain balanced evaluation.

### 3. Modeling Approach

* Constructed a machine learning pipeline using:

  * `StandardScaler` for feature normalization
  * `LogisticRegression` (default regularization settings)
* Fitted the model on the training dataset and evaluated on both train and test splits.

### 4. Evaluation Metrics

* Accuracy (Train: \~95.6%)
* Confusion Matrix
* Precision, Recall, F1-score
* False Alarm Rate
* ROC Curve and AUC (analyzed separately for training and testing data)

---

## Key Insights

* The model achieved high classification accuracy, suggesting good generalization.
* Most informative features included:

  * Bare Nuclei
  * Clump Thickness
  * Bland Chromatin
* ROC-AUC plots confirmed effective separation between benign and malignant cases.

---

## Tools and Technologies

* **Python**
* **Pandas**, **NumPy** for data handling
* **Scikit-learn** for modeling and metrics
* **Matplotlib**, **Seaborn** for visualization

---

## Conclusion

This analysis provides a reproducible and interpretable approach for diagnosing tumor status using logistic regression. The pipeline is adaptable to similar binary classification problems in the healthcare domain or beyond.

---
