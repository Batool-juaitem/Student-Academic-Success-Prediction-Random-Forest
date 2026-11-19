# Student Academic Success Prediction Using Random Forest

## 1. Project Overview
This project aims to predict students' academic outcomes using machine learning classification techniques.

The goal is to classify students into three categories:
- Graduate
- Dropout
- Enrolled

The main algorithm used is **Random Forest**, with other machine learning models used for comparison.

## 2. Dataset Information
The project uses the **Predict Students' Dropout and Academic Success** dataset from the UCI Machine Learning Repository.

**Dataset Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)

| Description | Value |
|---|---:|
| Total Records | 4,424 |
| Total Columns | 37 |
| Number of Classes | 3 |
| Missing Values | 0 |
| Duplicate Rows | 0 |

## 3. Data Analysis and Preparation
Exploratory Data Analysis (EDA) was performed to understand the dataset and identify important patterns.

The analysis included:
- Checking missing values and duplicate records.
- Analyzing target class distribution.
- Exploring dataset features.
- Creating charts and visualizations.

## 4. Machine Learning Models
Three classification algorithms were implemented:
- Random Forest
- Decision Tree
- Gradient Boosting

Random Forest was the main model, and its hyperparameters were adjusted to evaluate their effect on performance.

## 5. Model Performance Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Random Forest | 0.7672 | 0.7214 | 0.6802 | 0.6916 |
| Decision Tree | 0.6972 | 0.6378 | 0.6397 | 0.6385 |
| Gradient Boosting | 0.7593 | 0.7073 | 0.6813 | 0.6902 |

### Random Forest Optimization

| Metric | Before | After |
|---|---:|---:|
| Accuracy | 0.7672 | 0.7706 |
| Precision | 0.7214 | 0.7218 |
| Recall | 0.6802 | 0.6794 |
| F1-Score | 0.691
