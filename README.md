# Classification

Project Summary: Credit Card Default Prediction
Objective:
Developed a machine learning model to predict credit card default payment using the UCI Credit Card Default dataset with 30,000 samples and 24 features.

Data Preprocessing & EDA:
Exploratory Data Analysis (EDA):

Analyzed correlations using heatmaps and visualized trends for key features like LIMIT_BAL, PAY_*, and AGE against default status.

Used count, distribution, and box plots to understand data patterns.
Identified and visualized class imbalance in the target variable (default.payment.next.month), with 78% non-defaults and 22% defaults.
Data Cleaning:

No missing or duplicate values were detected.
Removed irrelevant features such as ID for model optimization.
Handled class imbalance through undersampling and SMOTE (oversampling).
Model Development & Evaluation:
Algorithms Used:

Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Performance Metrics:

Evaluated models using accuracy, precision, recall, and F1-score.

Results with original imbalanced data:
Logistic Regression: Accuracy: 81%, F1: 35.3%
Random Forest: Accuracy: 81.2%, F1: 45.4%

Results after undersampling:
Logistic Regression: Accuracy: 66.4%, F1: 65.2%
Random Forest: Accuracy: 68.8%, F1: 65.8%

Results with SMOTE (optimal performance):
Logistic Regression: Accuracy: 71.9%, F1: 71.9%
Decision Tree: Accuracy: 74.8%, F1: 75.3%
Random Forest: Accuracy: 84.3%, F1: 83.9%

Skills & Tools:
Libraries: Pandas, Seaborn, Matplotlib, Scikit-learn, Imbalanced-learn
Techniques: Data scaling (StandardScaler), feature engineering, balancing class distribution (undersampling, SMOTE)

Key Insights:
Random Forest Classifier performed best with 84.3% accuracy and 83.9% F1-score after balancing the dataset.

SMOTE improved model generalizability by addressing class imbalance effectively.

This project showcases proficiency in exploratory data analysis, handling imbalanced datasets, and implementing machine learning models with proper evaluation.



Project: Credit Card Fraud Detection Using Machine Learning
Objective:
Developed a machine learning model to detect fraudulent credit card transactions from highly imbalanced datasets.
Key Features:
Dataset: Worked with a publicly available credit card transactions dataset containing 284,807 records and 492 fraud cases.
Techniques:
Addressed data imbalance using SMOTE (Synthetic Minority Oversampling Technique) and undersampling.
Scaled transaction amounts using StandardScaler and removed duplicates for data preprocessing.
Algorithms Used:
Trained and evaluated multiple classifiers, including:
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Evaluation Metrics:
Compared models using accuracy, precision, recall, and F1-score to identify the best-performing model.
Key Contributions:
Data Preprocessing:
Handled imbalanced data distribution using oversampling and undersampling.
Performed feature scaling on transaction amounts and removed irrelevant features like time.
Model Development:
Achieved high-performance fraud detection using a Decision Tree Classifier.
Automated the prediction process with a saved model using Joblib.
Deployment:
Implemented real-time fraud detection for individual transactions using pre-trained models.
Tools & Technologies:
Python (Pandas, NumPy, Scikit-learn, Imbalanced-learn)
Joblib for model saving/loading
Google Colab for development and Google Drive for dataset storage.
Achievements:
Successfully balanced the dataset to enhance model performance in detecting minority fraud cases.
Improved recall to ensure high sensitivity in identifying fraudulent transactions.
