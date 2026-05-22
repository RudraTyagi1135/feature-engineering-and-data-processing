# 📊 Imbalanced Learning: Resampling Techniques & Model Behavior Analysis

A structured machine learning project focused on **handling class imbalance in classification systems** using oversampling and undersampling techniques.

This project emphasizes **model behavior, evaluation strategy, and trade-offs**, rather than relying on accuracy alone.

---

## 🚀 Project Overview

In real-world systems such as:

- Fraud detection  
- Healthcare risk prediction  
- Anomaly detection  

datasets are often **highly imbalanced**, leading to:

- Misleadingly high accuracy  
- Poor minority class detection  

This project investigates how **resampling strategies impact model performance and decision boundaries**.

---

## 🎯 Objectives

- Build a **baseline model on imbalanced data**
- Apply:
  - Oversampling techniques  
  - Undersampling techniques  
- Evaluate models using **class-sensitive metrics**
- Understand **trade-offs between methods**
- Move toward **decision-aware model evaluation**

---

## 📂 Project Structure

```bash
IMBALANCED_LEARNING/
│
├── 01_baseline_model_imbalanced_data.ipynb
├── 02_oversampling_smote_ros.ipynb
├── 03_undersampling_tomek_enn_ncr.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Experimental Design

### 1️⃣ Baseline Model (Imbalanced Data)

- Train model on skewed dataset  
- No resampling applied  

**Observation:**

- High accuracy  
- Extremely poor minority recall  

---

### 2️⃣ Oversampling Techniques

- Random OverSampling (ROS)  
- SMOTE (Synthetic Minority Over-sampling Technique)  

**Approach:**

- Increase minority class representation  
- Retrain model  

**Trade-offs:**

- Improved recall  
- Risk of overfitting (synthetic / duplicated data)  

---

### 3️⃣ Undersampling Techniques

- Tomek Links  
- Edited Nearest Neighbors (ENN)  
- Neighbourhood Cleaning Rule (NCR)  

**Approach:**

- Remove noisy and overlapping samples  
- Improve class separability  

**Trade-offs:**

- Cleaner decision boundaries  
- Loss of potentially useful data  

---

## 🧪 Evaluation Framework

Focus is on **decision-critical metrics**:

- Recall (minority class) → primary metric  
- Precision → controls false positives  
- F1-score → balance between precision and recall  
- Confusion Matrix → error distribution  

> Accuracy is intentionally avoided as a primary metric.

---

## 🧪 Workflow

```
Data → Imbalance Analysis → Resampling → Model Training → Evaluation → Comparison
```

---

## 📊 Key Observations

- Baseline models fail on minority class despite high accuracy  
- SMOTE improves recall but may introduce noise  
- ROS is simple but can bias models due to duplication  
- Undersampling improves class separation but reduces data  

---

## ⚠️ Limitations

- Synthetic dataset (limited real-world complexity)  
- No cross-validation  
- No hyperparameter tuning  
- Notebook-based (no reusable pipeline)  

---

## 🚀 Future Improvements (High Impact)

### 1️⃣ Evaluation Upgrade

- Precision-Recall Curve  
- PR-AUC (critical for imbalance)  
- Threshold tuning  

---

### 2️⃣ Pipeline Integration

- sklearn + imblearn Pipeline  
- Reproducible preprocessing + modeling  

---

### 3️⃣ System-Level Improvements

- Stratified K-Fold Cross Validation  
- Experiment tracking (MLflow)  
- Real-world dataset integration  

---

## 🛠️ Tech Stack

- Python  
- NumPy, Pandas  
- Scikit-learn  
- imbalanced-learn  
- Matplotlib / Seaborn  

---

## 🎯 What This Project Demonstrates

- Understanding of **class imbalance challenges**  
- Ability to evaluate models using **correct metrics**  
- Practical knowledge of **resampling techniques**  
- Awareness of **trade-offs in real-world ML systems**  

---

## 📌 Key Takeaway

Handling class imbalance is not a preprocessing step —  
it is a **core modeling decision that directly impacts system reliability**.

---

## 👤 Author

**Rudra Tyagi**  
ML Systems | MLOps | AI Infrastructure