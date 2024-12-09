# Cirrhosis Survival Prediction

This repository contains a machine learning project aimed at predicting the survival status of patients diagnosed with liver cirrhosis. Using a combination of data preprocessing techniques and machine learning models, this project provides a framework for accurate survival prediction based on clinical and laboratory features.

![score](https://i.imgur.com/kwgIPwj.png)

![addressing class imbalance](https://i.imgur.com/feojdk1.png)

---

## Introduction
Liver cirrhosis is a chronic condition that significantly impacts patient survival. This project leverages machine learning to classify survival status into three categories:
- **C**: Compensated Cirrhosis
- **D**: Decompensated Cirrhosis
- **CL**: Chronic Liver Disease

The goal is to provide an automated and efficient way to assist clinicians in decision-making and resource allocation.

---

## Dataset
### Source
The dataset includes clinical and laboratory data for patients diagnosed with liver cirrhosis.

### Structure
- **Training Data**: 224 samples with 19 features (including 'Status').
- **Test Data**: 88 samples with 18 features (excluding 'Status').

### Preprocessing
- Imputation of missing values using median values.
- One-hot encoding for categorical features.
- Balancing the target labels using SMOTE (Synthetic Minority Oversampling Technique).

---

## Methodology
### Steps
1. **Data Cleaning and Preprocessing**: Handled missing values and categorical encoding.
2. **Class Balancing**: Addressed label imbalance using SMOTE.
3. **Model Training and Evaluation**:
   - Logistic Regression
   - Random Forest
   - Support Vector Machine (SVM)
4. **Prediction**: Used the best-performing model to generate test predictions.

---

## Models Used
### Logistic Regression
- A simple baseline model offering interpretability.

### Random Forest
- Robust against overfitting and effective for non-linear relationships.

### Support Vector Machine (SVM)
- Versatile and effective in high-dimensional feature spaces.

---

## Results
### Model Performance
The models were evaluated on a validation set:
- **Random Forest** achieved the best results with an accuracy of **82%**, providing strong recall for the minority class ('CL').

### Test Predictions
Predictions for the test dataset were saved to a file: `test_predictions.csv`.

---