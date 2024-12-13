# News Topic Classification Using Naive Bayes and Logistic Regression

## Overview
This project classifies news articles into four categories: **World News**, **Sports**, **Business**, and **Tech**.  
The dataset includes:
- **Training Data**: 120,000 samples  
- **Testing Data**: 7,600 samples  
Both datasets are balanced across the categories.  

The goal is to preprocess the text data, extract features, and train models using **Naive Bayes** and **Logistic Regression** to achieve high classification performance.

---

## Features

### Text Preprocessing
- Removal of HTML tags and URLs.
- Tokenization, lemmatization, and stopwords removal.
- Custom filtering of extra common words.

### Visualization
- Word clouds for overall and category-specific analysis.

### Feature Engineering
- TF-IDF vectorization with tri-grams and feature selection.

### Model Training
- Hyperparameter tuning using `GridSearchCV`.
- Evaluation of models using **precision**, **recall**, and **F1-score**.

### Error Analysis
- Insights into misclassifications and overlapping categories.

---

### Logistic Regression
- Implemented in a `scikit-learn` Pipeline for ease of use.

---

## Results

| **Metric**     | **Testing Data** |
|----------------|------------------|
| **Precision**  | 85.00%           |
| **Recall**     | 84.82%           |
| **F1-Score**   | 84.90%           |

### Observations
- Misclassifications often occur between **Business** and **Tech** due to overlapping content.



## Installation

### Clone the Repository
```bash
git clone https://github.com/yourusername/news-topic-classification.git
cd news-topic-classification
