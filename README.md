
# Chronic Kidney Disease Prediction Using Classification Techniques

A machine learning project focused on predicting Chronic Kidney Disease (CKD) using patient medical data and classification algorithms in **Weka**.

---

## Project Overview

Chronic Kidney Disease (CKD) is a condition where the kidneys gradually lose their ability to function properly over time. Early detection is important because it can help prevent serious health complications.

The goal of this project was to analyze patient medical data, apply different classification algorithms, and compare their performance in predicting whether a patient has CKD.

## Dataset Description

The dataset used in this project is the [Chronic Kidney Disease Dataset](https://archive.ics.uci.edu/dataset/336/chronic+kidney+disease) from the UCI Machine Learning Repository.

| Dataset Information | Details |
|---------------------|---------|
| Source | UCI Machine Learning Repository |
| Total Records | 400 |
| Input Attributes | 24 |
| Target Variable | CKD / Not CKD |
| Task | Binary Classification |

### Dataset Features

The dataset contains several health-related attributes, including:

- Age
- Blood Pressure
- Specific Gravity
- Albumin
- Sugar Level
- Red Blood Cells
- Hemoglobin
- Hypertension
- Diabetes

These attributes provide medical information that can help identify patterns related to Chronic Kidney Disease.

## Problem Description

The objective of this project was to build classification models that predict whether a patient has Chronic Kidney Disease based on their medical information.

The target variable contains two categories:

- **ckd:** Patient has Chronic Kidney Disease
- **notckd:** Patient does not have Chronic Kidney Disease

## Classification Algorithms

Three classification algorithms were selected and applied using Weka.

| Algorithm | Description |
|-----------|-------------|
| K-Nearest Neighbors (KNN) | Classifies patients based on similar records in the dataset. |
| Decision Tree (J48) | Uses a tree structure to make predictions based on patient attributes. |
| Naive Bayes | Uses probability to predict which class a patient belongs to. |

These algorithms were used to compare different approaches to classification.

## Data Preprocessing

Before applying the classification algorithms, the dataset was prepared using Weka.

The preprocessing steps included:

1. **Handling Missing Values:** Using Weka filters to handle missing data.
2. **Data Conversion:** Converting the dataset into ARFF format.
3. **Attribute Verification:** Checking that attributes were correctly identified as numeric or nominal.

These steps helped prepare the dataset for classification.

## Project Objective

The project aimed to compare KNN, J48 Decision Tree, and Naive Bayes in predicting Chronic Kidney Disease.

By applying different classification techniques to the same dataset, the project explored how machine learning can be used to identify patterns in medical data and support disease prediction.

## Tools and Technologies

- **Weka** – Data preprocessing and classification
- **UCI Machine Learning Repository** – Dataset source
- **ARFF** – Dataset format used in Weka

## References

Rubini, L., Soundarapandian, P., & Eswaran, P. (2015). *Chronic Kidney Disease* [Dataset]. UCI Machine Learning Repository.

https://doi.org/10.24432/C5G020

---

**Project:** Chronic Kidney Disease Prediction | **Tool:** Weka | **Task:** Classification
