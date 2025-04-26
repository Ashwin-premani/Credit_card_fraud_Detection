#Credit Card Fraud Detection
Dataset: Credit Card Fraud Detection Dataset

Overview
This project focuses on developing an efficient classification model to detect fraudulent credit card transactions.
Due to the severe class imbalance in the dataset (fraudulent transactions are rare compared to genuine ones), special techniques were applied to address this imbalance.
The model is designed to minimize false positives while maintaining high overall accuracy.

Project Structure
data/ - Contains the dataset (not uploaded due to size/license; download from Kaggle)

notebooks/ - Jupyter notebooks for exploration, preprocessing, and model building

models/ - Saved models and evaluation metrics

README.md - Project overview and instructions

Problem Statement
Develop a classification model to efficiently detect fraudulent transactions.

Dataset Features include:

Transaction amount

Merchant details

Timestamps

(Transformed) anonymized variables (V1, V2, ..., V28)

Key Steps
1. Data Preprocessing
Handled missing values (if any).

Performed feature scaling on transaction amounts.

Created new engineered features:

Transaction frequency per user

Spending patterns based on transaction time

Location mismatch indicators (if available)

2. Handling Class Imbalance
Applied techniques like:

Oversampling (SMOTE - Synthetic Minority Oversampling Technique)

Undersampling the majority class

Hybrid approaches

3. Model Development
Trained and evaluated different classification models:

Logistic Regression

Random Forest

XGBoost

Neural Networks (optional)

Performed hyperparameter tuning for optimization.

4. Model Evaluation
Used metrics suitable for imbalanced data:

Precision

Recall

F1-Score

ROC-AUC Score

Confusion Matrix

Special focus on reducing False Positives to avoid blocking genuine users.

Results
Achieved high recall for fraud detection with minimal impact on precision.

Best-performing model details are provided in the final report notebook.

How to Run
Clone this repository:

bash
Copy
Edit
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection
Download the dataset from Kaggle and place it inside the data/ folder.

Install the required libraries:

bash
Copy
Edit
pip install -r requirements.txt
Run the notebooks step-by-step to explore, preprocess, train, and evaluate the models.

Requirements
Python 3.8+

pandas

scikit-learn

imbalanced-learn

matplotlib

seaborn

xgboost (optional)

(Install via requirements.txt.)

