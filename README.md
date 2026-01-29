# Task 5 – Train-Test Split & Evaluation Metrics (Heart Disease Dataset)

## Objective
This task focuses on understanding how to evaluate a Machine Learning classification model using:
- Train-Test Split
- Logistic Regression
- Evaluation Metrics (Accuracy, Precision, Recall)
- Confusion Matrix interpretation

Dataset Used: **Heart Disease Dataset**

---

## Objective
To build a basic classification model that predicts whether a person has heart disease and evaluate its performance using standard metrics.

---

## Tools & Libraries
- Python 3
- Pandas
- Scikit-learn

---

## Dataset
**Heart Disease Dataset**
- Rows: 1025
- Features: age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal, target 
- Target Column: `target`
  - `1` → Heart disease present
  - `0` → Heart disease absent

---

##  Steps Performed
### 1️ Data Loading
- Loaded dataset using Pandas.
- Checked missing values and dataset structure.

### 2️ Feature & Target Split
- `X` = all columns except target
- `y` = target column

### 3️ Train-Test Split
- Split dataset into:
  - Training set (80%)
  - Testing set (20%)
- Used `random_state=42` for reproducibility.

### 4️ Model Training
- Model used: **Logistic Regression**
- Trained using `model.fit(X_train, y_train)`

### 5️ Prediction & Evaluation
- Predictions made on test set.
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - Confusion Matrix

---

##  Results
| Metric | Value |
|--------|-------|
| Accuracy | **0.7951219512195122** |
| Precision | **0.7563025210084033** |
| Recall | **0.8737864077669902** |

### Confusion Matrix
| 73 | 29 |
|--------|-------|
| 13 | 90 |
