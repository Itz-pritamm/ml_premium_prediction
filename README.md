# Premium Prediction Using Machine Learning 

This project aims to predict health insurance premium amounts using Machine Learning (ML) .

## 🔹 Project Overview

- **Goal**: Predict insurance premium amounts based on user demographic and medical features.
- **Techniques Used**: Data cleaning, feature engineering, model training, and evaluation.

## 🔹 Data Preparation and EDA

- Handled missing (null) values appropriately.
- Brought data into a proper format using preprocessing steps.
- Used EDA to extract insights and detect issues affecting model performance.

## 🔹 Initial Model Performance

- Trained a machine learning model on the full dataset.
- Achieved **98% accuracy**, but observed a **30% average difference** between actual and predicted values.
- After analysis, the **age** column was found to be the main cause, especially for users aged 25 or younger.

## 🔹 Data Splitting Strategy

- Split data into two subsets:
  - **Young Group**: Age ≤ 25
  - **Rest Group**: Age > 25

- Trained separate models for each:
  - **Rest Group** model: Achieved **99% accuracy**
  - **Young Group** model: Initially only **60% accuracy**

## 🔹 Feature Enhancement

- Introduced a new feature: **Genetic Risk Score** (based on medical history).
- After adding this feature:
  - **Young Group** model improved from 60% to **98% accuracy**

## 🔹 Final Solution

- Developed a **two-model system**:
  - `model_young.joblib` for users aged ≤ 25
  - `model_rest.joblib` for users aged > 25
- Achieved high accuracy across both age groups.
- The model is ready to be deployed with a scalable prediction pipeline.

