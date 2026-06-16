# Breast Cancer Classification using Logistic Regression

## Overview

This project focuses on predicting whether a breast tumor is malignant or benign using Logistic Regression.

The goal was not only to build a classification model, but also to understand the evaluation metrics commonly used in classification problems such as Precision, Recall, F1 Score, ROC Curve, and ROC-AUC.

This project was completed as part of my Machine Learning learning journey while studying classification algorithms.

---

## Dataset

The dataset was loaded directly from Scikit-Learn:

```python
from sklearn.datasets import load_breast_cancer
```

The dataset contains various measurements computed from digitized images of breast masses.

### Target Classes

- 0 → Malignant
- 1 → Benign

---

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Project Workflow

1. Load Breast Cancer Dataset
2. Create DataFrame
3. Perform Basic EDA
4. Check Class Distribution
5. Train-Test Split
6. Feature Scaling using StandardScaler
7. Train Logistic Regression Model
8. Evaluate Model Performance
9. Plot ROC Curve
10. Calculate ROC-AUC Score
11. Perform Hyperparameter Tuning using GridSearchCV

---

## Exploratory Data Analysis

Some basic analysis was performed before training:

- Dataset shape and structure
- Data types
- Missing value check
- Target class distribution
- Correlation analysis
- Confusion Matrix visualization

The dataset was already clean and contained no missing values.

---

## Baseline Logistic Regression Results

### Accuracy

```text
97.90%
```

### Confusion Matrix

```text
[[53  2]
 [ 1 87]]
```

### Classification Report

| Metric | Score |
|----------|----------|
| Precision | 0.98 |
| Recall | 0.99 |
| F1 Score | 0.983 |

### ROC-AUC

```text
0.9955
```

---

## Hyperparameter Tuning

GridSearchCV was used to search for better combinations of:

- C
- Penalty
- Solver

The tuned model achieved performance similar to the baseline model.

### Tuned Model Results

| Metric | Score |
|----------|----------|
| Accuracy | 96.50% |
| F1 Score | 0.972 |
| ROC-AUC | 0.9957 |

---

## Observations

- Logistic Regression performed extremely well on this dataset.
- The model achieved nearly 98% accuracy on unseen test data.
- ROC-AUC was close to 1, indicating excellent class separation.
- Hyperparameter tuning did not significantly improve performance.
- The default Logistic Regression model already generalized very well.

One interesting observation was that the tuned model achieved a slightly higher ROC-AUC score, but a lower Accuracy and F1 Score compared to the baseline model.

---

## Key Concepts Practiced

- Logistic Regression
- Binary Classification
- Train-Test Split
- StandardScaler
- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC Curve
- ROC-AUC Score
- GridSearchCV
- Hyperparameter Tuning

---

## Future Improvements

Some ideas to extend this project:

- Support Vector Machines (SVM)
- Decision Trees
- Random Forest Classifier
- Feature Selection
- Cross Validation Comparison
- Model Deployment using Flask

---

## Author

**Krrish Rajput**

Machine Learning Learning Journey Project