# 💳 Credit Card Fraud Detection

A machine learning project that uses **Logistic Regression** to detect fraudulent credit card transactions from the popular Kaggle dataset.

## 📋 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Technologies Used](#technologies-used)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [License](#license)

## 🎯 Overview

This project implements a binary classification model to identify fraudulent credit card transactions. Due to the highly imbalanced nature of the dataset (frauds are rare), the model uses stratified sampling to maintain class distribution during training.

## 📊 Dataset

The project uses the **Credit Card Fraud Detection Dataset** from Kaggle.

- **Total Transactions**: 284,807
- **Fraudulent Transactions**: 492 (0.172%)
- **Features**: 30 (V1-V28 from PCA, Amount, Time)
- **Target**: Class (0 = Normal, 1 = Fraud)

### Download Dataset
Download the `creditcard.csv` file from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place it in the project root directory.

## ✨ Features

- ✅ Data preprocessing and exploration
- ✅ Stratified train-test split to handle class imbalance
- ✅ Logistic Regression classification
- ✅ Model evaluation with multiple metrics
- ✅ Confusion matrix visualization

## 🛠️ Installation

### Prerequisites
- Python 3.7+
- pip

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
```

2. **Install required packages**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

Or use requirements.txt:
```bash
pip install -r requirements.txt
```

3. **Download the dataset**
- Download `creditcard.csv` from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Place it in the project root directory

## 🚀 Usage

Run the main script:

```bash
python fraud_detection.py
```

### Expected Output
📊 Dataset Loaded!
Total rows: 284807
Fraud cases: 492

✅ Accuracy: 0.9992

🧾 Classification Report:
               precision    recall  f1-score   support

           0       1.00      1.00      1.00     56864
           1       0.82      0.65      0.73        98

    accuracy                           1.00     56962
   macro avg       0.91      0.83      0.86     56962
weighted avg       1.00      1.00      1.00     56962


📌 Confusion Matrix:
 [[56850    14]
 [   34    64]]
