# 🎬 Textual Data Analysis (IMDB Reviews)

A **Natural Language Processing (NLP) project** focused on analyzing **IMDB movie reviews** to extract insights using **text preprocessing, n-grams, and visualization techniques**.

This project demonstrates **end-to-end text data handling**, from raw review cleaning to **feature extraction and exploratory analysis**, along with **visual insights using word clouds and frequency distributions**.

---

## 🚀 Features

- 🧹 **Text preprocessing (cleaning, tokenization)**
- 🔤 **N-gram analysis (bi-grams / tri-grams)**
- ☁️ **WordCloud visualization (positive & negative reviews)**
- 📊 **Frequency-based textual insights**
- 🧠 **Sentiment-based filtering**
- 📈 **Exploratory Data Analysis (EDA) on text data**
- ⚡ **Jupyter Notebook-based workflow**

---

## 🧠 What This Project Demonstrates

This project highlights **core NLP and data analysis capabilities**:

- **Text preprocessing pipelines**
- **Tokenization and normalization techniques**
- **N-gram feature engineering**
- **Exploratory text analytics using Pandas**
- **Visualization using Matplotlib & WordCloud**
- **Handling real-world unstructured datasets**
- **Working inside Jupyter Notebook environments**

---

## 📂 Project Structure

```
TEXTUAL_DATA_ANALYSIS/
│
├── IMDB Dataset.csv        # Raw dataset (movie reviews)
├── movie_analysis.ipynb    # Main analysis notebook
├── requirements.txt        # Dependencies
│
├── .gitignore
├── README.md
│
└── .venv/                  # Virtual environment (local)
```

---

## ⚙️ Architecture Overview

The project follows a **structured NLP analysis pipeline**.

```
Raw Text Data (IMDB Dataset)
        │
        ▼
Data Cleaning
(remove noise, lowercase, etc.)
        │
        ▼
Tokenization
(split into words/tokens)
        │
        ▼
Feature Engineering
(n-grams, frequency counts)
        │
        ▼
Exploratory Analysis
(value_counts, distributions)
        │
        ▼
Visualization
(word clouds, patterns)
```

### Design Principles

- **Structured NLP workflow**
- **Clear separation of preprocessing and analysis**
- **Reproducible notebook-based pipeline**
- **Focus on interpretability and insights**

---

## 📊 Dataset Overview

The dataset consists of **IMDB movie reviews** with:

- Review text  
- Sentiment labels (**positive / negative**)  

### Key Characteristics

- Unstructured textual data  
- Binary sentiment classification  
- Real-world noisy text (punctuation, stopwords, etc.)  

---

## 🔍 Core Analysis Performed

### 1️⃣ Text Preprocessing

- Lowercasing  
- Removing special characters  
- Tokenization  
- Preparing clean text for analysis  

---

### 2️⃣ N-gram Analysis

- Generated **bi-grams / tri-grams**
- Identified:
  - Common phrases in reviews  
  - Repeated sentiment patterns  

Example logic:

```python
pd.Series(ngrams(df['tokenized_review'].sum(), 3)).value_counts()
```

---

### 3️⃣ WordCloud Visualization

**Positive Reviews**

- Extracted positive reviews  
- Generated WordCloud to visualize dominant terms  

```python
WordCloud().generate(" ".join(df[df['sentiment']=='positive']['review']))
```

**Negative Reviews**

- Filtered negative reviews  
- Visualized common negative expressions  

```python
WordCloud().generate(" ".join(df[df['sentiment']=='negative']['review']))
```

---

### 4️⃣ Exploratory Insights

- Most frequent words and phrases  
- Differences between positive and negative sentiment  
- Language patterns in user reviews  

---

## 🛠 Installation

### Clone repository

```bash
git clone https://github.com/your-username/textual_data_analysis.git
cd textual_data_analysis
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
movie_analysis.ipynb
```

---

## 📈 Potential Improvements

Future enhancements could include:

- Train sentiment classification models (**Logistic Regression / XGBoost / BERT**)
- Add advanced features (**TF-IDF, Word2Vec, FastText**)
- Convert notebook into **modular pipeline**
- Build **REST API (Flask / FastAPI)** for inference
- Deploy on **AWS (SageMaker / Lambda)**
- Add **real-time text processing pipelines**
- Implement **MLOps pipeline (MLflow, monitoring, drift detection)**

---

## 🧰 Tech Stack

| Technology | Purpose |
|-----------|--------|
| Python | Core programming |
| Pandas | Data manipulation |
| NLTK / Custom | Text processing |
| Matplotlib | Visualization |
| WordCloud | Text visualization |
| Jupyter Notebook | Development environment |

---

## 🎯 Learning Outcomes

This project helped build understanding of:

- **Natural Language Processing fundamentals**
- **Text preprocessing and feature engineering**
- **Exploratory analysis on unstructured data**
- **Visualization of textual patterns**
- **Preparing data for ML pipelines**

---

## 👤 Author

**Rudra**

B.Tech Final Year Student  
**ML Systems / MLOps Engineer**
