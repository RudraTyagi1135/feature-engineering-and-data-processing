# Feature Engineering and Data Processing

A master repository of machine learning projects focused on exploratory data analysis, preprocessing, feature engineering, class imbalance handling, and Scikit-learn pipeline design.

This repository is organized as a collection of focused notebook-based projects. Each folder represents a major stage of the machine learning workflow, and each subproject demonstrates a specific practical technique used to prepare data for reliable model development.

## Project Purpose

Real-world machine learning systems depend heavily on data quality, preprocessing choices, and feature design. This repository demonstrates practical techniques used before and during model development, including:

- Exploratory data analysis
- Data cleaning and standardization
- Feature transformation
- Feature scaling
- Missing value imputation
- Outlier and anomaly detection
- Class imbalance handling
- Feature discretization and binning
- Categorical encoding
- Scikit-learn pipeline construction
- Text preprocessing and NLP analysis

The goal is to move from isolated notebook experiments toward reliable, reusable, production-oriented ML preprocessing systems.

## Repository Structure

```text
feature-engineering-and-data-processing/
|
|-- exploratory_data_analysis/
|   |-- SMARTPHONE_DATA_CLEANING_PIPELINE/
|   |-- SMARTPHONE_EDA_PIPELINE/
|   |-- TEXTUAL_DATA_ANALYSIS/
|   `-- TITANIC_SURVIVAL_EDA/
|
|-- feature_engineering/
|   |-- FEATURE_ENGINEERING_AND_SKLEARN_PIPELINE/
|   `-- FEATURE_ENGINEERING_DISCRETIZATION_SYSTEMS/
|
|-- imbalance_handling/
|   `-- IMBALANCED_LEARNING_TECHNIQUE_ANALYSIS/
|
|-- preprocessing/
|   |-- DATA_TRANSFORMATION/
|   |-- FEATURE_SCALING_TECHNIQUES/
|   |-- MISSING_VALUE_IMPUTATION_TECHNIQUES/
|   `-- OUTLIER_DETECTION_TECHNIQUE/
|
`-- README.md
```

## Project Categories

## Exploratory Data Analysis

Projects under `exploratory_data_analysis/` focus on understanding datasets, identifying patterns, visualizing relationships, and preparing analytical insights before modeling.

### SMARTPHONE_DATA_CLEANING_PIPELINE

Transforms messy smartphone product specifications into a structured ML-ready dataset.

Covered topics:

- Raw data cleaning
- Regex-based feature extraction
- Semi-structured text parsing
- Smartphone hardware feature engineering
- Structured dataset generation

Main files:

- `data_cleaning.ipynb`
- `smartphones.csv`
- `smartphone_cleaned_v2.csv`

### SMARTPHONE_EDA_PIPELINE

Performs exploratory data analysis on cleaned smartphone data.

Covered topics:

- Brand analysis
- Price distribution
- Rating analysis
- Hardware feature analysis
- Feature availability analysis
- Visualization-driven insights

Main files:

- `smartphone_eda.ipynb`
- `smartphone_cleaned_v5.csv`

### TEXTUAL_DATA_ANALYSIS

Explores IMDB review text data using NLP preprocessing and visualization.

Covered topics:

- Text cleaning
- Tokenization
- N-gram analysis
- WordCloud visualization
- Sentiment-based text exploration

Main files:

- `movie_analysis.ipynb`
- `IMDB Dataset.csv`

### TITANIC_SURVIVAL_EDA

Performs structured exploratory analysis on the Titanic survival dataset.

Covered topics:

- Data inspection
- Missing value analysis
- Univariate analysis
- Bivariate analysis
- Correlation analysis
- Survival pattern discovery

Main files:

- `eda_titanic.ipynb`
- `train.csv`
- `test.csv`

## Preprocessing

Projects under `preprocessing/` focus on preparing raw or imperfect data for modeling through transformations, scaling, imputation, and anomaly handling.

### DATA_TRANSFORMATION

Explores feature transformation techniques used to improve data distribution and model compatibility.

Covered topics:

- Log transformation
- Reciprocal transformation
- Square root transformation
- Exponential transformation
- Polynomial feature engineering
- Distribution analysis using KDE and Q-Q plots

Main files:

- `feature_engineering_and_transformation_techniques.ipynb`
- `titanic_feature_transformation_analysis.ipynb`

### FEATURE_SCALING_TECHNIQUES

Demonstrates core scaling techniques and their impact on model readiness.

Covered topics:

- Min-Max scaling
- Standardization
- Before/after distribution visualization
- Scale-sensitive model behavior

Main files:

- `feature_scaling_minmax.ipynb`
- `feature_scaling_standardization.ipynb`

### MISSING_VALUE_IMPUTATION_TECHNIQUES

Compares missing value handling strategies using the Titanic dataset.

Covered topics:

- Missing value analysis
- Mean and median imputation
- KNN imputation
- Iterative imputation
- Pipeline-based imputation
- GridSearchCV integration

Main files:

- `01_missing_values_analysis_titanic.ipynb`
- `02_manual_missing_value_imputation_demo.ipynb`
- `03_knn_imputation_titanic_classification.ipynb`
- `04_iterative_imputation_random_forest_titanic.ipynb`
- `05_pipeline_imputation_with_gridsearch_titanic.ipynb`

### OUTLIER_DETECTION_TECHNIQUE

Demonstrates statistical and machine learning-based anomaly detection techniques.

Covered topics:

- Z-score outlier detection
- IQR-based outlier detection
- Isolation Forest
- KNN anomaly detection
- Local Outlier Factor
- DBSCAN

Main files:

- `outlier_detection_zscore_method.ipynb`
- `outlier_detection_iqr_method.ipynb`
- `multivariate_anomaly_detection_method.ipynb`

## Feature Engineering

Projects under `feature_engineering/` focus on transforming raw variables into useful model inputs and building reusable Scikit-learn preprocessing systems.

### FEATURE_ENGINEERING_AND_SKLEARN_PIPELINE

Builds reusable Scikit-learn preprocessing and modeling pipelines.

Covered topics:

- Custom Scikit-learn estimators
- `Pipeline`
- `ColumnTransformer`
- Ordinal encoding
- One-hot encoding
- Schema mismatch handling
- Unknown category handling
- Pipeline serialization

Main files:

- `01_custom_sklearn_estimator_and_model_evaluation.ipynb`
- `02_feature_engineering_pipeline_with_column_transformer.ipynb`
- `03_categorical_encoding_strategies_ordinal_vs_onehot.ipynb.ipynb`
- `pipe.pkl`

### FEATURE_ENGINEERING_DISCRETIZATION_SYSTEMS

Focuses on feature binning and discretization for improving model behavior, especially with linear models and non-linear relationships.

Covered topics:

- Manual binning
- Uniform binning
- Quantile binning
- `KBinsDiscretizer`
- One-hot encoding after binning
- Bias-variance trade-offs

Main files:

- `feature_binning_strategies.ipynb`
- `discretization_for_model_performance.ipynb`

## Imbalance Handling

Projects under `imbalance_handling/` focus on classification problems where one class is significantly underrepresented.

### IMBALANCED_LEARNING_TECHNIQUE_ANALYSIS

Analyzes classification behavior on imbalanced datasets and compares resampling strategies.

Covered topics:

- Baseline model behavior on imbalanced data
- Random oversampling
- SMOTE
- Tomek Links
- Edited Nearest Neighbors
- Neighbourhood Cleaning Rule
- Precision, recall, F1-score, and confusion matrix evaluation

Main files:

- `01-imbalanced-data-baseline-model-analysis.ipynb`
- `02-oversampling-methods-smote-ros-comparison.ipynb`
- `03-undersampling-methods-tomek-enn-ncr-analysis.ipynb`

## Common Workflow

Most subprojects follow this general workflow:

```text
Raw Data
   |
   v
Data Inspection
   |
   v
Cleaning / Preprocessing
   |
   v
Feature Engineering
   |
   v
Visualization / Evaluation
   |
   v
ML-ready Output or Insight
```

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- imbalanced-learn
- Matplotlib
- Seaborn
- Plotly
- Missingno
- WordCloud
- Jupyter Notebook

## Installation

Each subproject has its own `requirements.txt`. Install dependencies from the specific project you want to run.

Example:

```bash
cd feature_engineering/FEATURE_ENGINEERING_AND_SKLEARN_PIPELINE
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

For Linux or macOS:

```bash
source .venv/bin/activate
```

## Running a Project

Open the target subproject and start Jupyter Notebook:

```bash
jupyter notebook
```

Then run the notebooks listed in that subproject's README.

Example:

```bash
cd preprocessing/MISSING_VALUE_IMPUTATION_TECHNIQUES
jupyter notebook
```

## Current Architecture

This repository is currently notebook-first. It is useful for experimentation, learning, comparison, and documenting preprocessing behavior.

Current characteristics:

- Domain-grouped project folders
- Notebook-based workflows
- Local CSV datasets
- Independent subproject folders
- Per-project dependency files
- Some serialized model/pipeline artifacts
- No shared root package yet
- No root-level API service yet

## Production Upgrade Path

The natural next step is to convert the strongest workflows into a modular ML system.

Recommended target architecture:

```text
src/
|
|-- config/
|-- data/
|-- features/
|-- models/
|-- pipelines/
|-- api/
|-- logging/
`-- utils/
```

Recommended improvements:

- Add a shared `config.yaml`
- Move reusable logic from notebooks into Python modules
- Add data validation with Pydantic or Great Expectations
- Add structured logging
- Add experiment tracking with MLflow
- Add model and prediction logging
- Add FastAPI inference endpoints
- Store artifacts and datasets in AWS S3
- Package training jobs for AWS SageMaker
- Add Lambda-compatible lightweight inference where suitable
- Add Airflow DAGs for scheduled data and model workflows

## Deployment Direction

The long-term deployment direction should support:

- FastAPI for model inference
- AWS S3 for data and model artifacts
- AWS SageMaker for training and batch inference
- AWS Lambda for lightweight event-driven inference
- CloudWatch for logs and monitoring
- Airflow for orchestration

Any production inference service should log all predictions with:

- Request timestamp
- Model version
- Input schema version
- Prediction output
- Confidence or score where available
- Runtime errors or validation failures

## Learning Outcomes

This repository demonstrates practical understanding of:

- Data preprocessing fundamentals
- Feature engineering techniques
- Exploratory data analysis
- Scikit-learn pipeline design
- Model evaluation trade-offs
- Handling noisy, missing, imbalanced, and unstructured data
- Organizing ML projects by workflow stage
- Preparing notebook experiments for production ML systems

## Author

Rudra Tyagi

ML Systems | MLOps | AI Infrastructure
