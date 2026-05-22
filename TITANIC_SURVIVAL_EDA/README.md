# 🚢 Titanic Survival Analysis (Exploratory Data Analysis)

A **structured Exploratory Data Analysis (EDA) project** on the Titanic dataset to identify **survival patterns, feature relationships, and data-driven insights** using Python.

This project focuses on **data understanding, statistical exploration, and visualization-driven reasoning**, which are critical before building machine learning systems.

---

## 🚀 Features

- 📊 **Comprehensive univariate and bivariate analysis**
- 🔍 **Missing value and data quality assessment**
- 📈 **Correlation analysis using heatmaps**
- 🧠 **Feature-level insights for ML readiness**
- ⚡ **Notebook-based analytical workflow**
- 🧩 **Clear and interpretable visualizations**

---

## 🧠 What This Project Demonstrates

This project highlights the following **data analysis and ML foundation skills**:

- **Structured Exploratory Data Analysis (EDA)**
- **Statistical reasoning on real-world datasets**
- **Feature relationship analysis**
- **Data cleaning and preprocessing strategies**
- **Visualization-driven insights using Matplotlib & Seaborn**
- **Preparation for machine learning pipelines**

---

## 📂 Project Structure

```
TITANIC_SURVIVAL_EDA/
│
├── eda_titanic.ipynb      # Main analysis notebook
├── train.csv              # Training dataset
├── test.csv               # Test dataset
├── requirements.txt       # Project dependencies
├── README.md              # Project documentation
├── .gitignore
└── .venv/                 # Virtual environment (excluded from Git)
```

---

## ⚙️ Architecture Overview

The project follows a **data analysis pipeline**.

```
Raw Dataset (train.csv / test.csv)
        │
        ▼
Data Inspection & Cleaning
        │
        ▼
Missing Value Handling
        │
        ▼
Exploratory Analysis
(Univariate / Bivariate)
        │
        ▼
Correlation Analysis
        │
        ▼
Insights for ML Modeling
```

### Design Principles

- **Step-by-step analytical workflow**
- **Data-driven reasoning before modeling**
- **Clear separation of analysis stages**
- **Reproducible notebook-based pipeline**

---

## 🔍 Analysis Workflow

### 1️⃣ Data Inspection

- Dataset shape and schema  
- Feature types (numerical / categorical)  
- Initial data quality checks  

---

### 2️⃣ Missing Value Analysis

- Identification of null values  
- Detection of high-missing columns (e.g., Cabin)  
- Strategy for handling missing data  

---

### 3️⃣ Univariate Analysis

- Distribution of **Age, Fare**  
- Passenger class frequency  
- Survival distribution  

---

### 4️⃣ Bivariate Analysis

- Survival vs Gender  
- Survival vs Passenger Class  
- Survival vs Age groups  

---

### 5️⃣ Correlation Analysis

- Feature relationships using heatmaps  
- Identification of influential variables  

---

## 📊 Key Insights

- **Gender is the strongest predictor**  
  Female passengers had significantly higher survival rates  

- **Socio-economic status matters**  
  First-class passengers were more likely to survive  

- **Fare correlates with survival**  
  Higher ticket fares show positive association  

- **Age influence is moderate**  
  Younger passengers had slightly better survival probability  

---

## 🛠 Installation

### Clone repository

```bash
git clone https://github.com/your-username/titanic-survival-eda.git
cd titanic-survival-eda
```

### Create virtual environment (optional)

```bash
python -m venv .venv
```

### Activate environment (Windows)

```bash
.venv\Scripts\activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

```bash
jupyter notebook eda_titanic.ipynb
```

---

## 📈 Potential Improvements

Future enhancements could include:

- Feature engineering (age groups, family size)
- Build baseline ML models (Logistic Regression, Random Forest)
- Model evaluation (ROC-AUC, Precision-Recall)
- Convert notebook into **modular ML pipeline**
- Deploy as **interactive dashboard (Streamlit)**

---

## 🧰 Tech Stack

| Technology | Purpose |
|-----------|--------|
| Python | Programming language |
| Pandas | Data processing |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Development environment |

---

## 🎯 Learning Outcomes

This project helped build understanding of:

- **Exploratory Data Analysis workflows**
- **Feature-level reasoning before modeling**
- **Handling missing and noisy data**
- **Visualization-driven insights**
- **Foundations for ML pipeline development**

---

## 👤 Author

**Rudra**

ML Systems Engineer | MLOps | AI Infrastructure  
B.Tech Final Year Student