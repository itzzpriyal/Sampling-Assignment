#  Sampling Techniques on Imbalanced Credit Card Data

##  Overview
This project studies the effect of different sampling techniques on an imbalanced credit card fraud dataset. The objective is to understand how sampling impacts the accuracy of multiple machine learning models and to identify the best sampling–model combinations.

---

## 📂 Dataset
- **Dataset**: Credit Card Fraud Detection  
- **Target Column**: `Class`  
  - `0` → Normal transaction  
  - `1` → Fraudulent transaction  
- The dataset is highly imbalanced, with very few fraud cases.

---

## ⚙️ Methodology

### 1️ Data Splitting
- The dataset is split into training and testing sets using **stratified sampling**.
- This preserves the original class distribution in both sets.

### 2️ Data Balancing
- **SMOTE (Synthetic Minority Oversampling Technique)** is applied **only on the training data**.
- This prevents data leakage and avoids unrealistic accuracy values.

### 3️ Sampling Techniques
Five different sampling strategies are applied to the balanced training data:
1. Simple Random Sampling  
2. Stratified Sampling  
3. Systematic Sampling  
4. Cluster Sampling  
5. Full SMOTE-based Sampling  

---

##  Machine Learning Models
The following five models are used:
- Logistic Regression  
- Decision Tree  
- Random Forest  
- K-Nearest Neighbors (KNN)  
- Naive Bayes  

These models represent linear, tree-based, ensemble, distance-based, and probabilistic learning approaches.

---

##  Evaluation Metric
- **Accuracy** is used to evaluate model performance.
- Results are compared in a tabular format to determine the best sampling technique for each model.

---

##  Key Observations
- Different models perform best under different sampling techniques.
- Sampling plays a crucial role in handling imbalanced datasets.
- Applying sampling only on training data helps prevent overfitting.

---

##  Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Imbalanced-learn  

---

##  Conclusion
This project highlights the importance of proper sampling techniques when working with imbalanced datasets. A careful combination of sampling methods and machine learning models leads to more reliable and realistic results.
