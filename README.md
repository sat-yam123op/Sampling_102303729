# Sampling Techniques on Imbalanced Credit Card Dataset

**Name:** Sneha Goswami  
**Roll Number:** 102303723  

---

## Problem Statement
The objective of this assignment is to understand the importance of sampling techniques in handling imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

A highly imbalanced credit card fraud dataset was provided. Such imbalance can significantly degrade classification performance. The task was to balance the dataset using multiple sampling techniques and evaluate their impact on different machine learning models.

---

## Methodology

**Dataset:**  
The credit card dataset was downloaded from the provided GitHub source and loaded into a pandas DataFrame. The dataset contains a severe class imbalance between fraudulent and non-fraudulent transactions.

**Sampling Techniques Applied:**  
Five sampling techniques were used to create balanced datasets:

- Random UnderSampling (Sampling1)  
- Random OverSampling (Sampling2)  
- SMOTE (Sampling3)  
- SMOTE-Tomek (Sampling4)  
- NearMiss (Sampling5)  

**Machine Learning Models:**  
Five classification models were trained on each sampled dataset:

- Logistic Regression (M1)  
- Decision Tree (M2)  
- Random Forest (M3)  
- K-Nearest Neighbors (M4)  
- Gaussian Naive Bayes (M5)  

**Evaluation Procedure:**  
- Each sampled dataset was split into training and testing sets  
- Models were trained on the training data  
- Accuracy was computed on the test data  
- Results were compared across all model–sampling combinations  

---

## Results

Accuracy comparison of models across sampling techniques:

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|-----------|-----------|-----------|-----------|-----------|
| Logistic Regression | 33.33 | 91.92 | 91.92 | 92.79 | 50.00 |
| Decision Tree | 50.00 | 98.69 | 98.25 | 97.97 | 16.67 |
| Random Forest | 33.33 | 100.00 | 99.34 | 99.55 | 16.67 |
| KNN | 33.33 | 98.47 | 83.84 | 86.71 | 83.33 |
| Naive Bayes | 33.33 | 74.67 | 87.77 | 82.66 | 33.33 |

**Best Sampling Technique per Model:**

- Logistic Regression → Sampling4 (SMOTE-Tomek)  
- Decision Tree → Sampling2 (Random OverSampling)  
- Random Forest → Sampling2 (Random OverSampling)  
- KNN → Sampling2 (Random OverSampling)  
- Naive Bayes → Sampling3 (SMOTE)  

--- 

## Conclusion
This study demonstrates the importance of sampling strategies when working with imbalanced datasets. Different sampling techniques affect model performance differently, and no single method is optimal for all models. Selecting an appropriate sampling strategy can substantially improve classification accuracy in fraud detection tasks.

--- 
