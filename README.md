🚀 Credit Card Fraud Detection

Dataset: Credit Card Fraud Detection - Kaggle

📖 Overview
This project builds an efficient classification model to detect fraudulent credit card transactions.
The dataset is highly imbalanced, so specialized techniques are applied to ensure high fraud detection rates while minimizing false positives.

🗂️ Project Structure
bash
Copy
Edit
credit-card-fraud-detection/
├── data/             # Dataset files (download manually)
├── models/           # Saved trained models
├── notebooks/        # Jupyter Notebooks for EDA, preprocessing, and modeling
├── requirements.txt  # Python libraries needed
├── README.md         # Project information
├── .gitignore        # Files and folders to be ignored by Git
🛠️ Steps Followed
1. Data Preprocessing
Checked for missing values.

Scaled Amount feature.

Engineered new features:

Transaction frequency by user.

Spending patterns based on time.

Location mismatch indicators (if data available).

2. Handling Class Imbalance
Techniques used:

SMOTE (Synthetic Minority Oversampling)

Random Undersampling

Combination strategies.

3. Model Building
Models trained and evaluated:

Logistic Regression

Random Forest

XGBoost

(Optionally) Neural Networks

Performed hyperparameter tuning for better accuracy.

4. Model Evaluation
Focused on Recall, Precision, and F1-Score.

Plotted ROC-AUC curves.

Analyzed Confusion Matrix to minimize false positives.

📈 Results
Achieved a strong balance between recall and precision.

Best model selection based on minimizing false positives while maintaining high detection accuracy.

🧪 How to Run Locally
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection
Install the required libraries:

bash
Copy
Edit
pip install -r requirements.txt
Download the dataset from Kaggle and place it into the data/ folder.

Run the Jupyter notebook:

bash
Copy
Edit
jupyter notebook notebooks/your_notebook_name.ipynb
⚙️ Requirements
Python 3.8+

numpy

pandas

scikit-learn

imbalanced-learn

matplotlib

seaborn

xgboost

jupyter

joblib

(Install with pip install -r requirements.txt)

📜 License
This project is licensed under the MIT License.
