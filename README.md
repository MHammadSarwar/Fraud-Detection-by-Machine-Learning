# Credit Card Fraud Detection

![GitHub](https://img.shields.io/badge/Language-Python-blue)
![GitHub](https://img.shields.io/badge/Library-Scikit_Learn-orange)
![GitHub](https://img.shields.io/badge/Model-Random_Forest-green)

This project focuses on detecting fraudulent credit card transactions using machine learning. It involves handling class imbalance, feature engineering, and training a Random Forest model to achieve high recall and precision. The final model achieves an F1-score of **0.86**, effectively identifying fraud while minimizing false positives.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)

---

## Project Overview
Credit card fraud is a significant issue in the financial industry, costing billions of dollars annually. This project aims to build a machine learning model that can accurately detect fraudulent transactions. The model is trained on a highly imbalanced dataset and optimized to maximize recall while maintaining reasonable precision.

---

## Dataset
The dataset used in this project is the [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) from Kaggle. It contains anonymized credit card transactions, with features `V1-V28` (PCA-transformed), `Time`, `Amount`, and the target variable `Class` (1 for fraud, 0 for non-fraud).

---

## Methodology
1. **Data Preprocessing**:
   - Handled missing values (none found).
   - Scaled the `Amount` and `Time` features.
   - Addressed class imbalance using **SMOTE** (Synthetic Minority Oversampling Technique).

2. **Feature Engineering**:
   - Created new features like `Hour`, `Time_Since_Last_Transaction`, and `Amount_Scaled`.
   - Selected top features using **Random Forest feature importance**.

3. **Model Training**:
   - Trained a **Random Forest** model with hyperparameter tuning.
   - Achieved an F1-score of **0.86** and a recall of **0.83**.

4. **Evaluation**:
   - Evaluated the model using **precision**, **recall**, **F1-score**, and **ROC-AUC**.
   - Visualized results using a **confusion matrix** and feature importance plot.

---

## Results
- **F1-Score**: 0.86
- **Recall**: 0.83
- **Precision**: 0.89
- **ROC-AUC**: 0.98

### Confusion Matrix
![image](https://github.com/user-attachments/assets/c8028ed7-a234-48c2-a184-5368bebcf1d6)


---

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
