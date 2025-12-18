# Bank_Account_Fraud_Detection
## Academic Machine Learning Project (Kaggle-Style)

This repository presents an end-to-end **academic machine learning study** on bank account fraud detection using the **Bank Account Fraud Dataset (NeurIPS 2022)**.  
The project follows a structured, reproducible workflow aligned with **Kaggle-style data science practices** and academic reporting standards.

**Dataset:** Bank Account Fraud Dataset – NeurIPS 2022 (Kaggle)

---

## Abstract

Financial fraud detection is a critical problem in modern banking systems due to its direct financial and security impacts. In this project, we analyze a real-world fraud detection dataset and implement a complete machine learning pipeline including preprocessing, dimensionality reduction, unsupervised learning, supervised classification, automated model benchmarking, and cross-validation. The primary objective is to study model performance under class imbalance and evaluate the effectiveness of preprocessing and validation strategies.

---

## Research Objectives

- Analyze a real-world, highly imbalanced fraud detection dataset  
- Apply principled preprocessing and feature engineering techniques  
- Explore data structure using unsupervised learning  
- Train and evaluate supervised classification models  
- Benchmark multiple algorithms efficiently  
- Ensure reliable evaluation using cross-validation  

---

## Dataset Description

The dataset consists of anonymized bank customer records with a binary target variable indicating whether an account is fraudulent.

**Key characteristics:**
- Mixed numerical and categorical features  
- Missing values and outliers  
- Severe class imbalance (fraud vs non-fraud)  

These properties make the dataset well-suited for academic study and real-world fraud detection analysis.

---

## Repository Structure

```text
├── model.ipynb        # Complete experimental pipeline and results
├── Academic_report.pdf          # Academic report (theoretical background)
├── README.md          # Project documentation
├── requirements.txt           # requirements for Run
```
---
## Methodology 

### 1. Data Preprocessing
To ensure model robustness, the following steps are applied:

- Handling missing values
- Outlier detection and removal
- Encoding categorical variables
- Feature standardization
- Train/test split
- Class balancing using SMOTE

### 2. Dimensionality Reduction
Dimensionality reduction is applied prior to clustering and visualization to:

- Reduce computational overhead
- Improve cluster separability
- Enable low-dimensional visualization

### 3. Unsupervised Learning: K-Means Clustering
K-Means clustering is used as an exploratory analysis tool:

- Identifies latent data groupings
- Evaluates preprocessing quality
- Enables visual inspection of cluster separation

Clustering results are used for analysis only and not direct prediction.

### 4. Supervised Learning: K-Nearest Neighbors (KNN)
KNN is implemented as a baseline supervised classifier:

- Distance-based decision rule
- Sensitive to feature scaling
- Simple and interpretable

Predictions are made using majority voting among the nearest neighbors.

### 5. Automated Model Benchmarking: LazyPredict
To align with Kaggle-style experimentation, LazyPredict is used to benchmark approximately 29 classification algorithms:

- Rapid comparison of model performance
- Identification of strong baseline models
- Reduced manual experimentation

Due to computational cost, benchmarking is performed on a reduced dataset.

### 6. Model Evaluation: Cross-Validation
Reliable evaluation is ensured using:
- K-Fold Cross-Validation
- Stratified K-Fold Cross-Validation

Benefits include:
- Reduced overfitting
- Stable performance estimates
- Fair model comparison

---
## How to Run
1. Clone the Repository
2. Install dependencies
``` pip install -r requirements.txt ```
3. Run the notebook:
``` jupyter notebook model.ipynb ```

--- 
Author

Erfan Najafi
Faculty of Mathematics and Computer Science
Amirkabir University of Technology (Tehran Polytechnic)
