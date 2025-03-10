Credit Card Fraud Detection 🕵️‍♂️💳
This Jupyter Notebook demonstrates a credit card fraud detection model using Logistic Regression. It includes data exploration, preprocessing, model training, and evaluation.

📊 Dataset Overview
Dataset: creditcard.csv
Size: 284,807 transactions, 31 features
Features: Time, Amount, Class, and V1 to V28 (PCA-transformed)
Class Distribution: Highly imbalanced (few fraud cases)
🔍 Exploratory Data Analysis (EDA)
Statistical summary (df.describe().T)
Fraud vs. non-fraud pie chart
Heatmap for feature correlation
⚙️ Data Preprocessing
Removed duplicate rows
Split data into training (75%) and test (25%) sets
Defined features (X) and target variable (y)
🤖 Model Training
Used Logistic Regression
Faced a ConvergenceWarning (suggesting more iterations or data scaling)
📈 Model Evaluation
Confusion Matrix:
Train set: [[212348, 89], [137, 220]]
Test set: [[70784, 32], [37, 79]]
Classification Report:
Accuracy: 99.9%
Recall for fraud cases is relatively low
Final Accuracy:
Train: 99.89%
Test: 99.90%
💾 Model Saving
Saved using joblib (model_filename.pkl) for future use
⚠️ Observations & Next Steps
The dataset is highly imbalanced, affecting fraud detection
High accuracy may be misleading due to class imbalance
Model can be improved using:
Oversampling fraud cases (SMOTE)
Anomaly detection techniques
Other ML models like Random Forest or Neural Networks
