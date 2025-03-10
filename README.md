# Credit-Card-Fraud-Detection
A credit card fraud detection project using Logistic Regression. It includes data exploration, preprocessing, model training, and evaluation. The dataset has 284,807 transactions, with an imbalanced class distribution (few fraud cases).
The PDF contains a Jupyter Notebook output related to a machine learning project, specifically a credit card fraud detection task. Here’s what I observed:

Dataset Information:

The dataset (creditcard.csv) has 284,807 rows and 31 columns.
Columns include Time, Amount, Class, and V1 to V28 (likely features from PCA).
No missing values in the dataset.
Exploratory Data Analysis (EDA):

df.describe().T shows summary statistics of the dataset.
A pie chart was plotted to show fraud vs. non-fraud transactions.
A Seaborn heatmap was used to visualize feature correlations.
Data Preprocessing:

Removed duplicate rows.
Split the dataset into features (X) and target variable (y).
Used train_test_split() to create training and test sets.
Model Training:

Used Logistic Regression for fraud detection.
Encountered a ConvergenceWarning, suggesting that more iterations or data scaling was needed.
Model Evaluation:

Confusion Matrix results:
Train set: [[212348, 89], [137, 220]]
Test set: [[70784, 32], [37, 79]]
Classification Report:
High accuracy (~99.9%) but relatively low recall for fraud detection.
Accuracy Scores:
Train: 99.89%
Test: 99.90%
Model Saving:

Saved the trained model using joblib (model_filename.pkl).
Observations:
The dataset is highly imbalanced, as there are far fewer fraud cases.
The high accuracy might be misleading due to class imbalance.
The model might benefit from resampling techniques like oversampling fraud cases or using anomaly detection methods.
Let me know if you need further insights! 🚀
