
# Chronic Kidney Disease Prediction Using Machine Learning

A machine learning project focused on predicting Chronic Kidney Disease (CKD) using classification algorithms in **Weka**.

## Project Overview

Chronic Kidney Disease (CKD) is a condition where the kidneys gradually lose their ability to filter waste and excess fluids from the blood. Early detection is important because it can help prevent serious health complications.

This project uses machine learning classification techniques to predict whether a patient has CKD based on medical information.

Three classification algorithms were applied and compared:
- K-Nearest Neighbors (KNN)
- Decision Tree (J48)
- Naive Bayes

The models were evaluated using 10-fold cross-validation to compare their performance.

## Dataset Description

The dataset used in this project is the [Chronic Kidney Disease Dataset](https://archive.ics.uci.edu/dataset/336/chronic+kidney+disease) from the UCI Machine Learning Repository.

| Dataset Information | Details |
|---------------------|---------|
| Source | UCI Machine Learning Repository |
| Total Records | 400 |
| Input Features | 24 |
| Target Variable | CKD / Not CKD |
| CKD Cases | 250 |
| Non-CKD Cases | 150 |
| Task | Binary Classification |

### Dataset Features

The dataset includes several medical attributes, such as:

- Age
- Blood Pressure
- Specific Gravity
- Albumin
- Sugar Level
- Red Blood Cells
- Hemoglobin
- Serum Creatinine
- Hypertension
- Diabetes

These features help identify patterns associated with Chronic Kidney Disease.

## Data Preprocessing

The dataset was prepared using Weka before applying the classification algorithms.

The preprocessing steps included:

1. **Handling Missing Values:** Used Weka's ReplaceMissingValues filter to replace missing numeric values with the mean and nominal values with the mode.
2. **Normalization:** Applied the Normalize filter to scale numeric attributes between 0 and 1.
3. **Data Format:** Loaded the dataset in ARFF format using Weka Explorer.
4. **Evaluation:** Used 10-fold cross-validation to evaluate all three classifiers.

## Classification Algorithms

Three machine learning classification algorithms were implemented using Weka.

| Algorithm | Description |
|-----------|-------------|
| K-Nearest Neighbors (IBk, K=3) | Classifies patients based on the three most similar records. |
| Decision Tree (J48) | Uses a tree structure to classify patients based on medical attributes. |
| Naive Bayes | Uses probability to predict whether a patient has CKD. |

## Results and Model Comparison

All three models achieved accuracy of 95% or higher.

| Algorithm | Accuracy | False Negatives | False Positives | Kappa Statistic |
|-----------|----------|-----------------|-----------------|-----------------|
| KNN (IBk, K=3) | **97.75%** | 9 | 0 | 0.9526 |
| Decision Tree (J48) | 96.75% | **6** | 7 | 0.9306 |
| Naive Bayes | 95.00% | 20 | 0 | 0.8961 |

### Key Findings

- **KNN (IBk, K=3)** achieved the highest accuracy at 97.75%, correctly classifying 391 out of 400 patient records.
- **Decision Tree (J48)** achieved 96.75% accuracy and had the fewest false negatives (6), meaning it missed fewer actual CKD cases.
- **Naive Bayes** achieved 95.00% accuracy and correctly identified all 150 non-CKD patients.
- All three models performed better than the majority-class baseline of 62.5%.

Although KNN achieved the highest overall accuracy, J48 performed better in minimizing false negatives, which is important when predicting medical conditions.

## Conclusion

This project demonstrated how machine learning classification techniques can be used to identify patterns in medical data and predict Chronic Kidney Disease.

KNN achieved the highest overall accuracy, while Decision Tree (J48) produced fewer false negatives and provided more interpretable results.

The findings show the potential of machine learning in supporting early disease detection. However, further testing with larger and more diverse datasets would be needed before using these models in real clinical settings.

## Tools and Technologies

- **Weka** – Data preprocessing, classification, and evaluation
- **ARFF** – Dataset format
- **UCI Machine Learning Repository** – Dataset source

## Project Report

The complete project report includes detailed methodology, preprocessing steps, Weka results, confusion matrices, and model comparisons.

[View Full Project Report](CKD_Final_Paper.pdf)

## References

Rubini, L., Soundarapandian, P., & Eswaran, P. (2015). *Chronic Kidney Disease* [Dataset]. UCI Machine Learning Repository.

https://doi.org/10.24432/C5G020
