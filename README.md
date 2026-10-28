# CreditWise — Loan Approval Prediction System

A machine learning project that predicts loan approval outcomes using applicant information and compares multiple classification algorithms to identify the best-performing model.

## Project Overview

CreditWise uses machine learning to analyze applicant data and predict whether a loan application is likely to be approved. The project covers data preprocessing, exploratory data analysis, feature engineering, model training, and performance evaluation.

The objective is to build a reliable classification pipeline and understand how different machine learning algorithms perform on loan approval prediction.

## Features

- Data cleaning and missing-value handling
- Exploratory Data Analysis (EDA)
- Categorical feature encoding
- Numerical feature scaling
- Machine learning model training and comparison
- Evaluation using accuracy, precision, recall, and F1-score
- Confusion matrix analysis
- Selection of the best-performing classifier

## Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Scikit-learn | Preprocessing, model training, and evaluation |
| Matplotlib / Seaborn | Data visualization |

## Machine Learning Models

The project evaluates the following classification algorithms:

1. **Naïve Bayes** — selected as the best-performing model based on the reported evaluation results.
2. **Logistic Regression** — baseline classification model.
3. **K-Nearest Neighbors (KNN)** — distance-based classification model.

## Project Workflow

1. **Data Loading:** Load the loan application dataset and inspect its structure.
2. **Exploratory Data Analysis:** Examine feature distributions, missing values, and relationships between variables.
3. **Data Preprocessing:** Impute missing numerical values using the median and categorical values using the mode.
4. **Feature Engineering:** Encode categorical variables and scale numerical features where appropriate.
5. **Model Training:** Train Naïve Bayes, Logistic Regression, and KNN classifiers.
6. **Model Evaluation:** Compare the models using standard classification metrics and confusion matrices.
7. **Model Selection:** Identify Naïve Bayes as the best-performing model based on the recorded results.

## Results

The selected Naïve Bayes model achieved the following evaluation metrics:

| Metric | Score |
|---|---:|
| Accuracy | 86.50% |
| Precision | 80.36% |
| Recall | 73.77% |
| F1-Score | 76.92% |

### Confusion Matrix

The recorded confusion matrix is:

| | Predicted Negative | Predicted Positive |
|---|---:|---:|
| Actual Negative | 128 | 11 |
| Actual Positive | 16 | 45 |

The matrix shows 128 true negatives, 11 false positives, 16 false negatives, and 45 true positives, using the project's original label ordering.

**Note:** The interpretation of positive and negative classes depends on how loan approval labels are encoded in the dataset.

## Installation and Setup

### Prerequisites

- Python 3.9 or later
- pip
- Git

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd CreditWise
```

Replace the repository URL and directory name with your actual values.

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On macOS or Linux:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

### 4. Run the project

If the project is implemented in a Jupyter Notebook:

```bash
jupyter notebook
```

Open the project's
