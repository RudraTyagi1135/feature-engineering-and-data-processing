# 🚀 Feature Engineering & Scikit-learn Pipeline Systems

A structured machine learning project focused on building **production-oriented feature engineering pipelines** using Scikit-learn.

This project emphasizes **pipeline correctness, reproducibility, and real-world preprocessing challenges**, moving beyond isolated notebook experimentation.

---

## 🚀 Project Overview

This repository demonstrates how to design robust ML preprocessing systems by covering:

- Feature engineering pipelines using `ColumnTransformer`  
- Custom model development using Scikit-learn internals  
- Categorical encoding strategies and trade-offs  
- Handling real-world issues like schema mismatch and unseen categories  

The goal is to move from:

> **Notebook experimentation → Pipeline-based ML engineering**

---

## 🎯 Objectives

- Build:
  - reusable and robust preprocessing pipelines  

- Understand:
  - Scikit-learn internals (custom estimators)  
  - encoding strategies and their impact  

- Handle:
  - unknown categories  
  - schema inconsistencies  
  - real-world inference challenges  

---

## 🧠 Core Concepts Covered

### Feature Engineering Systems

- Feature engineering as a system design problem  
- Consistent preprocessing across training and inference  

---

### Scikit-learn Pipelines

- `Pipeline` for sequential transformations  
- `ColumnTransformer` for column-wise operations  
- Reproducible preprocessing workflows  

---

### Custom Estimators

- `BaseEstimator`  
- `ClassifierMixin`  
- Implementation of:
  - `fit()`  
  - `predict()`  

---

### Categorical Encoding

- Ordinal Encoding vs One-Hot Encoding  
- Handling:
  - ordered categories  
  - nominal variables  

---

## 📂 Project Structure

```
FEATURE_ENGINEERING_AND_SKLEARN_PIPELINE/
│
├── data/
│   ├── cars.csv
│   └── customer.csv
│
├── 01_custom_sklearn_estimator_and_model_evaluation.ipynb
├── 02_feature_engineering_pipeline_with_column_transformer.ipynb
├── 03_categorical_encoding_strategies_ordinal_vs_onehot.ipynb
│
├── pipe.pkl
│
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

---

## ⚙️ Implementation Breakdown

### 1️⃣ Custom Estimator & Model Evaluation

- Builds custom models using:
  - `BaseEstimator`  
  - `ClassifierMixin`  

- Implements:
  - `fit()`  
  - `predict()`  

**Key Insight:**

- Understanding internals is critical for debugging and extending ML systems  

---

### 2️⃣ Feature Engineering Pipeline (ColumnTransformer)

- Uses:
  - `ColumnTransformer`  
  - `Pipeline`  

- Combines:
  - OneHotEncoding  
  - OrdinalEncoding  
  - Numerical features  

**Key Insight:**

- Eliminates column-order dependency and ensures production-safe preprocessing  

---

### 3️⃣ Categorical Encoding Strategies

- Compares:
  - Ordinal Encoding  
  - One-Hot Encoding  

- Handles:
  - ordered vs unordered categories  

**Key Insight:**

- Encoding directly impacts model performance and interpretability  

---

## 📊 Dataset Description

### cars.csv

| Feature        | Description              |
|----------------|--------------------------|
| brand          | Car manufacturer         |
| km_driven      | Distance driven          |
| fuel           | Fuel type                |
| owner          | Ownership history        |
| selling_price  | Target variable          |

---

## 📦 Pipeline Artifact

### `pipe.pkl`

- Serialized preprocessing + model pipeline  
- Reusable for inference  
- Demonstrates model persistence  

---

## ⚠️ Real-World Pitfalls Addressed

This project explicitly handles:

- Column mismatch errors  
- Shape mismatch in encoders  
- Unknown categories during inference  
- Loss of DataFrame structure  
- Incorrect use of `.toarray()`  

---

## 🧩 Design Principles

- Explicit column selection (no index-based dependency)  
- Separation of:
  - raw data  
  - transformed data  

- Use of:
  - `ColumnTransformer`  
  - `Pipeline`  

- Reproducible preprocessing  

---

## ⚠️ Limitations

- No full end-to-end training pipeline with cross-validation  
- No experiment tracking (MLflow, etc.)  
- Limited dataset complexity  
- No deployment layer  

---

## 🔮 Future Improvements

- Add:
  - end-to-end ML pipeline notebook  
  - cross-validation (KFold)  
  - evaluation metrics (RMSE, R²)  

- Integrate:
  - XGBoost / advanced models  

- Add:
  - experiment tracking  
  - deployment layer (API + inference pipeline)  

---

## 🛠 Installation

### Clone repository

```bash
git clone https://github.com/RudrTyagi1135/feature_engineering_pipeline.git
cd FEATURE_ENGINEERING_AND_SKLEARN_PIPELINE
```

### Create virtual environment

```bash
python -m venv .venv
.venv\Scripts\activate      # Windows
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
jupyter notebook
```

Run notebooks in order:

1. `01_custom_sklearn_estimator_and_model_evaluation.ipynb`  
2. `02_feature_engineering_pipeline_with_column_transformer.ipynb`  
3. `03_categorical_encoding_strategies_ordinal_vs_onehot.ipynb`  

---

## 📊 Outputs

- Reusable preprocessing pipelines  
- Encoding strategy comparison  
- Custom estimator implementation  
- Pipeline serialization artifact  

---

## 🎯 What This Project Demonstrates

- Strong understanding of feature engineering systems  
- Ability to design production-ready preprocessing pipelines  
- Knowledge of Scikit-learn internals  
- Handling of real-world ML pipeline issues  

---

## 📌 Next Step

- Build:
  - end-to-end ML pipeline with model training  

- Add:
  - deployment (FastAPI / Streamlit)  
  - data validation layer  

---

## 👤 Author

**Rudra Tyagi**

ML Systems | MLOps | AI Infrastructure