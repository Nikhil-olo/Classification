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



Project Summary credit card fraud detection using a highly imbalanced dataset. Here's a concise overview of the work and the key takeaways that can be highlighted in your resume:

Project Overview
Objective: Detect fraudulent transactions in a credit card dataset while improving key evaluation metrics like precision, recall, and F1-score.
Dataset: Credit card transactions containing 284,807 rows and 31 features, including anonymized transaction details (V1 to V28), Amount, and the Class label (0: Normal, 1: Fraudulent).
Challenges:
Highly imbalanced data: ~99.8% transactions are normal, while ~0.2% are fraudulent.
Maintaining high recall and F1-score without compromising precision.

Key Steps and Techniques

Data Preprocessing:
Normalized the Amount column using StandardScaler.
Removed the Time column as it was not relevant for modeling.
Handled duplicate data to reduce redundancy.

Class Imbalance Management:
Explored undersampling and oversampling techniques:
Undersampling: Reduced majority class to match the minority class (473 samples each), balancing the dataset.
Oversampling: Could be applied using methods like SMOTE for better results.

Machine Learning Models:
Used the following classifiers to compare performance:
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Evaluated models using metrics like:
Accuracy: Overall correctness of predictions.
Precision: Fraction of correctly predicted fraud cases among all predicted fraud cases.
Recall: Ability to detect actual fraudulent transactions.
F1-Score: Harmonic mean of precision and recall.
Performance Results (Initial Imbalanced Dataset):

Random Forest Classifier performed best:
Accuracy: 99.95%
Precision: 90.7%
Recall: 74.7%
F1-Score: 81.9%
Future Steps:

Implement oversampling techniques like SMOTE to enhance recall and precision.
Perform hyperparameter tuning for improved performance.
Key Results and Learnings
Successfully addressed the data imbalance issue and demonstrated the importance of metrics like precision, recall, and F1-score over accuracy in imbalanced datasets.
Highlighted the trade-offs between different models and metrics.
Built an efficient fraud detection pipeline using various preprocessing techniques and machine learning algorithms.
