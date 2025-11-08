# Fetal Health Prediction

## Overview
This project aims to classify fetal health conditions based on cardiotocography (CTG) data using machine learning techniques. The classification identifies whether a fetus is in a **Normal**, **Suspect**, or **Pathological** state based on multiple biophysical parameters recorded during pregnancy.

The notebook implements a structured pipeline involving data preprocessing, exploratory data analysis, model training, performance evaluation, and result interpretation.

---

## Objectives
- To analyze fetal health data and detect key indicators of fetal distress.
- To build predictive models capable of classifying fetal health conditions with high accuracy.
- To evaluate and compare multiple machine learning algorithms using standard metrics.

---

## Dataset
The dataset contains fetal cardiotocography features such as:
- Baseline fetal heart rate
- Accelerations and decelerations
- Uterine contractions
- Variability metrics  
- Fetal movement indicators

The target variable represents three classes:
1. **Normal**
2. **Suspect**
3. **Pathological**

---

## Methodology

### 1. Data Loading and Preprocessing
- Data loaded from a CSV file using `pandas`.
- Checked for missing or inconsistent values.
- Standardization or normalization applied where necessary.
- Label encoding performed on the target variable.

### 2. Exploratory Data Analysis (EDA)
- Statistical summary and correlation analysis.
- Visualization of class distribution and feature relationships using **Matplotlib** and **Seaborn**.

### 3. Model Building
Implemented and compared multiple classification algorithms:
- Logistic Regression  
- Random Forest Classifier  
- XGBoost Classifier  

### 4. Model Evaluation
Performance measured using:
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

The **XGBoost Classifier** achieved the best performance, with approximately **96% accuracy** and **0.96 weighted F1 score**.

---

## Results
- The XGBoost model demonstrated superior classification performance across all key metrics.
- Random Forest and Logistic Regression models performed well but were slightly less accurate.
- The model effectively differentiates between the three fetal health categories.

---

## Dependencies
Ensure the following Python libraries are installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
