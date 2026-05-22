# 📱 Smartphone Data Preprocessing Pipeline

A **feature engineering and data preprocessing pipeline** that transforms **raw smartphone specifications** into a fully **structured, ML-ready dataset**.

This project focuses on extracting structured features from **semi-structured product data**, a common real-world challenge in **data engineering and ML systems**.

---

## 🚀 Features

- 🧹 **Cleaning messy and inconsistent raw data**
- 🔍 **Regex-based parsing of complex specification fields**
- ⚙️ **Feature engineering from unstructured text**
- 📊 **Creation of 24 structured features from raw input**
- 🤖 **ML-ready dataset generation**
- 📦 **End-to-end reproducible preprocessing pipeline**

---

## 🧠 What This Project Demonstrates

This project highlights the following **data engineering and ML foundation skills**:

- **Feature engineering from semi-structured data**
- **Regex-based parsing for real-world datasets**
- **Designing preprocessing pipelines for ML workflows**
- **Handling noisy, inconsistent, and mixed-format data**
- **Transforming raw data into structured analytical features**
- **Building data pipelines for downstream ML systems**

---

## 📂 Project Structure

```
SMARTPHONE_DATA_CLEANING_PIPELINE/
│
├── data_cleaning.ipynb            # Main preprocessing pipeline
├── smartphones.csv                # Raw dataset
├── smartphone_cleaned_v2.csv      # Cleaned dataset (output)
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Architecture Overview

The project follows a **data preprocessing pipeline architecture**.

```
Raw Data (smartphones.csv)
        │
        ▼
Data Ingestion (Pandas)
        │
        ▼
Cleaning & Standardization
        │
        ▼
Feature Extraction (Regex Parsing)
        │
        ▼
Feature Engineering
        │
        ▼
Structured Dataset (smartphone_cleaned_v2.csv)
```

### Design Principles

- **Structured transformation pipeline**
- **Separation of cleaning and feature extraction**
- **ML-ready feature design**
- **Reproducible workflow**

---

## 📌 Problem Context

The raw dataset contains:

- Mixed **text + numeric values**  
- Multiple features embedded in single columns  
- Inconsistent formatting across rows  

### Objective

Convert semi-structured product data into a **fully structured dataset** suitable for:

- Machine Learning  
- Analytics  
- Recommendation systems  

---

## 🔄 Pipeline Workflow

### 1️⃣ Data Ingestion

```python
df = pd.read_csv('smartphones.csv')
```

---

### 2️⃣ Cleaning & Normalization

- Removed symbols (₹, noise text)  
- Standardized inconsistent formats  
- Cleaned categorical values  

---

### 3️⃣ Feature Engineering (Core Strength)

Extracted structured features from raw text fields:

#### 📡 Connectivity Features
- `has_5g`
- `has_nfc`
- `has_ir_blaster`

#### ⚙️ Processor Features
- `processor_name`
- `processor_brand`
- `num_cores`
- `processor_speed`

#### 🔋 Battery Features
- `battery_capacity`
- `fast_charging`

#### 🧠 Memory Features
- `ram_capacity`
- `internal_memory`
- `extended_memory`

#### 📱 Display Features
- `screen_size`
- `refresh_rate`
- `resolution`

#### 📷 Camera Features
- `num_rear_cameras`
- `num_front_cameras`
- `primary_camera_rear`
- `primary_camera_front`

#### 🏷️ Additional Features
- `brand_name`
- `price`
- `rating`
- `os`

---

### 4️⃣ Handling Data Irregularities

- Managed inconsistent patterns across rows  
- Extracted values from noisy text  
- Ignored non-parsable fragments  

---

### 5️⃣ Data Type Conversion

- Numerical → `int` / `float`  
- Boolean → `0 / 1`  
- Ensured full ML compatibility  

---

### 6️⃣ Export Final Dataset

```python
export_df.to_csv('smartphone_cleaned_v2.csv', index=False)
```

---

## 📊 Output Dataset

Final dataset contains **24 structured features**:

| Category | Features |
|----------|---------|
| Basic | price, rating, brand_name |
| Connectivity | has_5g, has_nfc, has_ir_blaster |
| Processor | processor_brand, speed, cores |
| Battery | capacity, fast_charging |
| Memory | RAM, internal, extended |
| Display | size, resolution, refresh_rate |
| Camera | rear/front count + MP |

---

## 🛠 Installation

```bash
git clone https://github.com/your-username/smartphone-data-cleaning-pipeline.git
cd smartphone-data-cleaning-pipeline

python -m venv .venv

# Windows
.venv\Scripts\activate

# Mac/Linux
source .venv/bin/activate

pip install -r requirements.txt
```

---

## ▶️ Running the Project

```bash
jupyter notebook
```

Open:

```
data_cleaning.ipynb
```

---

## 📈 Use Cases

- 📊 Feature engineering pipelines  
- 🤖 ML model training (price prediction, ranking)  
- 📱 Recommendation systems  
- 📉 Product analytics  

---

## ⚠️ Limitations

- Regex-based parsing (sensitive to new formats)  
- No schema validation  
- Notebook-based (not production-ready)  
- Hardcoded parsing logic  

---

## 📈 Potential Improvements

Future enhancements could include:

- Convert into **modular pipeline (`src/` architecture)**  
- Add **data validation (Great Expectations / Pydantic)**  
- Introduce **logging and error handling**  
- Build **ML model on cleaned dataset**  
- Deploy as **API (FastAPI + AWS)**  
- Integrate into **MLOps pipeline**  

---

## 🎯 Learning Outcomes

This project helped build understanding of:

- **Feature engineering from unstructured data**
- **Designing preprocessing pipelines**
- **Handling real-world noisy datasets**
- **Preparing data for ML systems**
- **Structured data transformation workflows**

---

## 👤 Author

**Rudra Tyagi**

ML Systems Engineer | MLOps | AI Infrastructure  
B.Tech Final Year Student