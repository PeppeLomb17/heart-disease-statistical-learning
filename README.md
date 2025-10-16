# Heart Disease Prediction – Statistical Learning Project

**Author:** Giuseppe Lombardia  

---

## 1. Overview
This repository contains the complete project developed for the *Statistical Learning* course.  
The work focuses on the prediction of **heart disease** using classical and modern supervised learning models.  
All code, results and visualizations are included within the attached PDF report.

---

## 2. Objective
The goal of this project is to explore and compare different statistical learning methods to predict the presence of **cardiovascular disease**, using a real-world dataset derived from the **Cleveland Heart Disease dataset**.

The analysis aims to:
- Identify relevant predictors of heart disease.  
- Compare model performance across multiple techniques.  
- Evaluate diagnostic accuracy, sensitivity, and specificity.

---

## 3. Methods and Models
The project applies three main classification algorithms:

| Model | Description |
|--------|--------------|
| **Logistic Regression** | Baseline interpretable model for binary classification. |
| **Random Forest** | Ensemble learning method to capture non-linear relationships. |
| **Neural Network (nnet)** | Feed-forward network with tuned hidden layers. |

Each model is evaluated using:
- Confusion matrix  
- Accuracy, Precision, Sensitivity, Specificity  
- ROC curve and AUC  

---

## 4. Datasets
The analysis uses four CSV files, representing different dataset splits and preprocessing steps.

| File | Description |
|------|--------------|
| `heart_attack_train.csv` | Training set (60%) |
| `heart_attack_validation.csv` | Validation set (20%) |
| `heart_attack_test.csv` | Test set (20%) |
| `final data frame.csv` | Combined dataset after preprocessing |

All datasets include features such as:
- Age, sex, resting blood pressure, cholesterol, fasting blood sugar, resting ECG, maximum heart rate, exercise-induced angina, and others.

---

## 5. Report
The full R code, detailed results, plots, and interpretations are contained in the report:

📄 [`report/Statistical_Learning_GiuseppeLombardia.pdf`](report/Statistical_Learning_GiuseppeLombardia.pdf)

Sections include:
1. Exploratory Data Analysis (EDA)  
2. Model training and tuning  
3. Validation and testing  
4. Model comparison and discussion  

---

## 6. R Dependencies
To reproduce the analysis, install the following R packages:

```r
install.packages(c("readr","dplyr","ggplot2","caret","nnet",
                   "randomForest","psych","pROC","corrplot","GGally","gridExtra"))
A full list is also included in dependencies.md.

heart-disease-statistical-learning/
│
├─ data/
│   ├─ heart_attack_train.csv
│   ├─ heart_attack_validation.csv
│   ├─ heart_attack_test.csv
│
|- results/
|   └─ final data frame.csv
│
├─ report/
│   └─ Statistical_Learning_GiuseppeLombardia.pdf
│
├─ dependencies.md
├─ .gitignore
├─ LICENSE
└─ README.md
