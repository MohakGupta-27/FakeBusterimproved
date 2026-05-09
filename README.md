# Fake News Detection using Machine Learning & Ensemble Learning

## Overview

Fake news and misinformation on social media platforms have become a major global concern. This project presents a robust Fake News Detection System using Machine Learning, Natural Language Processing (NLP), and Ensemble Learning techniques to automatically classify news articles as **Real** or **Fake**.

The system applies advanced text preprocessing, TF-IDF feature extraction, and multiple classification models including:

- Naive Bayes
- Support Vector Machine (SVM)
- Feedforward Neural Network (FNN)
- Long Short-Term Memory (LSTM)
- Proposed Stacking Classifier (Random Forest + XGBoost + Logistic Regression)

The proposed Stacking Classifier achieved an accuracy of **99.81%**, outperforming all standalone models.

---

# Features

- Automated Fake News Classification
- NLP-based Text Preprocessing
- TF-IDF Feature Engineering
- Comparative Analysis of ML & DL Models
- Ensemble Learning using Stacking Classifier
- Confusion Matrix Visualization
- Accuracy & Performance Comparison Charts
- Scalable architecture for real-world deployment

---

# Tech Stack

## Programming Language
- Python 3

## Libraries & Frameworks
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- NLTK
- XGBoost
- Matplotlib
- Seaborn

---

# Dataset

The dataset consists of two CSV files:

| Dataset | Description |
|---|---|
| Fake.csv | 23,502 fake news articles |
| True.csv | 21,417 true news articles |

## Dataset Attributes
- Title
- Text
- Subject
- Date

---

# Project Workflow

## 1. Data Preprocessing
- Convert text to lowercase
- Remove punctuation and special characters
- Remove extra whitespaces
- Merge article title and content
- Text cleaning and normalization

## 2. Feature Extraction
TF-IDF Vectorization is used to convert textual content into numerical feature vectors.

## 3. Model Training

### Classical ML Models
- Naive Bayes
- Support Vector Machine (SVM)

### Deep Learning Models
- Feedforward Neural Network (FNN)
- LSTM Network

### Proposed Ensemble Model
- Random Forest
- XGBoost
- Logistic Regression (Meta Learner)
- Stacking Classifier

## 4. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# Model Performance

| Model | Accuracy | F1-Score |
|---|---|---|
| Stacking Classifier | 99.81% | 99.81% |
| SVM | 99.43% | 99.41% |
| Feedforward Neural Network | 99.22% | 99.19% |
| Naive Bayes | 95.62% | 95.42% |
| LSTM | 90.94% | 89.59% |

---

# Proposed Stacking Architecture

The core innovation of this project is the **Stacking Classifier Ensemble Model**.

## Base Learners
- Random Forest Classifier
- XGBoost Classifier

## Meta Learner
- Logistic Regression

The ensemble approach combines the strengths of multiple models to improve prediction robustness and reduce misclassification.

---

# Results

- Achieved **99.81% accuracy**
- Only **17 misclassifications** on the test dataset
- Better generalization than standalone models
- High precision and recall for both fake and real news detection

---

# Future Enhancements

- Integration with BERT and Transformer models
- Multilingual fake news detection
- Real-time social media monitoring
- Multimodal detection using images/videos
- Explainable AI for model transparency
- Adversarial fake news detection

---

# Repository Structure

```bash
Fake-News-Detection/
│
├── dataset/
│   ├── Fake.csv
│   └── True.csv
│
├── notebooks/
│   └── fake_news_detection.ipynb
│
├── models/
│   └── saved_models/
│
├── outputs/
│   ├── confusion_matrix/
│   └── accuracy_graphs/
│
├── requirements.txt
├── README.md
└── app.py
```

---

# Installation

```bash
git clone https://github.com/your-username/Fake-News-Detection.git
cd Fake-News-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the project:

```bash
python app.py
```

---

# Key Learning Outcomes

- Applied NLP techniques for text classification
- Built and evaluated multiple ML/DL models
- Implemented Ensemble Learning using Stacking
- Performed comparative analysis of classification algorithms
- Improved understanding of misinformation detection systems

---

# Contributors

- Mohak Gupta — Model Development & Comparative Analysis
- Shreya Gupta — PPT & Research Work
- Shaan Mathur — Literature Review & Documentation

---

# References

- Kaggle Fake News Dataset
- Scikit-learn Documentation
- TensorFlow Documentation
- Research papers on Fake News Detection, NLP, and Ensemble Learning
