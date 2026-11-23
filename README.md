# Sentiment Classification of Malay-English Code-Switched Text on Threads

## 1. Project Overview

This project focuses on sentiment classification of Malay-English code-switched text collected from public posts on Threads.

The objective is to classify text into four sentiment categories:
- Positive
- Negative
- Neutral
- Mixed

## 2. Dataset

The dataset contains 750 text samples.

- Training data: 600 samples (80%)
- Testing data: 150 samples (20%)
- Input feature: `CLEANED-COMMENT`
- Target label: `ANALYSIS SENTIMENT`

## 3. Methodology

The project uses a supervised machine learning approach.

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert text into numerical features.

Five model configurations are evaluated:

1. Multinomial Naive Bayes (Baseline)
2. Logistic Regression
3. Logistic Regression with Balanced Class Weights
4. Linear Support Vector Machine (SVM)
5. Linear SVM with Balanced Class Weights

## 4. Evaluation Metrics

The models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 5. Visualizations

The project includes three visualizations:

- `accuracy_comparison.png` – Accuracy comparison of five models.
- `performance_comparison.png` – Precision, Recall and F1-Score comparison.
- `confusion_matrices.png` – Confusion matrices for all five models.

## 6. Development Environment

- Python 3.13.16
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- NumPy 2.5.4

## 7. How to Run

Install the required libraries:

pip install -r requirements.txt

Run the Python script:

```bash
python sentiment_analysis.py
```

## 8. Project Files

- `sentiment_analysis.py` – Main Python implementation.
- `accuracy_comparison.png` – Accuracy visualization.
- `performance_comparison.png` – Performance metrics visualization.
- `confusion_matrices.png` – Confusion matrix visualization.
- `dataset/Threads_Sentiment_Dataset_Cleaned.csv` – Cleaned dataset used for sentiment classification.
- `requirements.txt` – List of required Python libraries and versions.
