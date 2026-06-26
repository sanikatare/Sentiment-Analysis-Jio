# Customer Sentiment Analysis for Jio Digital using Machine Learning

## Overview

This project performs **Sentiment Analysis** on customer reviews using **Natural Language Processing (NLP)** and **Machine Learning**. The objective is to classify customer reviews into sentiment categories such as **Positive**, **Negative**, and **Neutral** after applying comprehensive text preprocessing and feature engineering techniques.

The notebook demonstrates an end-to-end machine learning workflow, including data cleaning, exploratory data analysis, text preprocessing, vectorization, model training, evaluation, and sentiment prediction.

Although the project focuses on **Jio Digital** customer reviews, it is designed so that it can also work with similar product or service review datasets.

---

## Features

- Complete NLP preprocessing pipeline
- Text cleaning and normalization
- Stopword removal
- Lemmatization
- Exploratory Data Analysis (EDA)
- Feature extraction using:
  - Count Vectorizer
  - TF-IDF Vectorizer
- Multiple Machine Learning models
- Model performance comparison
- Classification metrics
- Confusion Matrix
- Sentiment prediction for custom input text

---

## Project Workflow

```
Dataset
    │
    ▼
Data Cleaning
    │
    ▼
Text Preprocessing
    │
    ▼
Exploratory Data Analysis
    │
    ▼
Feature Engineering
    │
    ▼
Text Vectorization (TF-IDF)
    │
    ▼
Train-Test Split
    │
    ▼
Machine Learning Models
    │
    ▼
Evaluation
    │
    ▼
Prediction
```

---

## Dataset

The notebook expects the Kaggle dataset:

**Flipkart Product Reviews with Sentiment Dataset**

Expected filename:

```
Dataset-SA.csv
```

If the dataset is unavailable, the notebook can fall back to a small synthetic Jio Digital review dataset for demonstration purposes.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn

---

## Machine Learning Pipeline

### 1. Data Loading

- Load customer review dataset
- Handle missing values
- Remove duplicate records

### 2. Text Preprocessing

The review text undergoes multiple preprocessing steps:

- Lowercase conversion
- URL removal
- HTML tag removal
- Emoji removal
- Punctuation removal
- Number removal
- Special character removal
- Tokenization
- Stopword removal
- Lemmatization

---

### 3. Exploratory Data Analysis

The notebook includes visualizations and analysis for:

- Sentiment distribution
- Review length analysis
- Word frequency
- General dataset statistics

---

### 4. Feature Engineering

The project converts textual data into numerical vectors using:

- Count Vectorizer
- TF-IDF Vectorizer

TF-IDF is selected for final model training because it emphasizes informative words while reducing the influence of highly frequent terms.

---

### 5. Train-Test Split

The processed dataset is divided into:

- 80% Training Data
- 20% Testing Data

A stratified split is used to preserve class distribution.

---

### 6. Machine Learning Models

Multiple classification algorithms are trained and evaluated to compare performance.

Examples include:

- Multinomial Naive Bayes
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest (depending on notebook execution)

---

### 7. Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Classification Report
- Confusion Matrix

---

### 8. Prediction

The trained model can predict sentiment for new customer reviews entered by the user.

Example:

```
Input:
"The internet speed is excellent and customer support is very helpful."

Prediction:
Positive
```

---

## Project Structure

```
Customer-Sentiment-Analysis-Jio-Digital/

│
├── Customer_Sentiment_Analysis_Jio_Digital.ipynb
├── Dataset-SA.csv
├── README.md
├── .gitignore
└── requirements.txt (optional)
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/customer-sentiment-analysis-jio-digital.git
```

Navigate into the project:

```bash
cd customer-sentiment-analysis-jio-digital
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## Required Libraries

```python
pandas
numpy
matplotlib
seaborn
nltk
scikit-learn
```

---

## Results

The notebook demonstrates:

- Cleaned and normalized review text
- Feature extraction using TF-IDF
- Training of multiple machine learning models
- Performance comparison
- Sentiment prediction on unseen reviews

---

## Learning Outcomes

This project demonstrates practical implementation of:

- Natural Language Processing (NLP)
- Text preprocessing techniques
- Feature engineering
- TF-IDF vectorization
- Machine Learning classification
- Model evaluation
- Customer sentiment prediction

---

## Future Improvements

Potential enhancements include:

- Deep Learning models (LSTM, GRU)
- Transformer-based models (BERT)
- Real-time sentiment prediction API
- Interactive Streamlit dashboard
- Word Clouds
- Hyperparameter tuning
- Model deployment using Flask or FastAPI
- Docker containerization

---
