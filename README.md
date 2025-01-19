<!DOCTYPE html>
<html>
<head>
    <title>Credit Card Projects Overview</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f8f9fa;
            color: #343a40;
            margin: 0;
            padding: 0 20px;
        }
        header {
            background-color: #007bff;
            color: white;
            padding: 20px 10px;
            text-align: center;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        section {
            background: #ffffff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            padding: 20px;
        }
        h1, h2, h3 {
            color: #007bff;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #007bff;
            color: white;
        }
        .key-insight {
            background-color: #e9f7ff;
            border-left: 5px solid #007bff;
            padding: 10px;
            margin: 10px 0;
        }
        a {
            color: #007bff;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>Credit Card Projects Overview</h1>
        <p>Detailed exploration of credit card default prediction and fraud detection.</p>
    </header>

    <section>
        <h2>Project 1: Credit Card Default Prediction</h2>
        <h3>Objective</h3>
        <p>Developed a machine learning model to predict credit card default payment using the UCI Credit Card Default dataset with 30,000 samples and 24 features.</p>

        <h3>Data Preprocessing & EDA</h3>
        <ul>
            <li><strong>Exploratory Data Analysis (EDA):</strong></li>
            <ul>
                <li>Analyzed correlations using heatmaps and visualized trends for key features like <code>LIMIT_BAL</code>, <code>PAY_*</code>, and <code>AGE</code> against default status.</li>
                <li>Used count, distribution, and box plots to understand data patterns.</li>
                <li>Identified and visualized class imbalance in the target variable (<code>default.payment.next.month</code>): 78% non-defaults and 22% defaults.</li>
            </ul>
            <li><strong>Data Cleaning:</strong></li>
            <ul>
                <li>No missing or duplicate values were detected.</li>
                <li>Removed irrelevant features such as <code>ID</code> for model optimization.</li>
                <li>Handled class imbalance through undersampling and SMOTE (oversampling).</li>
            </ul>
        </ul>

        <h3>Model Development & Evaluation</h3>
        <h4>Algorithms Used</h4>
        <ul>
            <li>Logistic Regression</li>
            <li>Decision Tree Classifier</li>
            <li>Random Forest Classifier</li>
        </ul>

        <h4>Performance Metrics</h4>
        <table>
            <tr>
                <th>Data Handling</th>
                <th>Algorithm</th>
                <th>Accuracy</th>
                <th>F1-Score</th>
            </tr>
            <tr>
                <td>Original Imbalanced</td>
                <td>Logistic Regression</td>
                <td>81%</td>
                <td>35.3%</td>
            </tr>
            <tr>
                <td>Original Imbalanced</td>
                <td>Random Forest</td>
                <td>81.2%</td>
                <td>45.4%</td>
            </tr>
            <tr>
                <td>After Undersampling</td>
                <td>Logistic Regression</td>
                <td>66.4%</td>
                <td>65.2%</td>
            </tr>
            <tr>
                <td>After Undersampling</td>
                <td>Random Forest</td>
                <td>68.8%</td>
                <td>65.8%</td>
            </tr>
            <tr>
                <td>With SMOTE</td>
                <td>Logistic Regression</td>
                <td>71.9%</td>
                <td>71.9%</td>
            </tr>
            <tr>
                <td>With SMOTE</td>
                <td>Decision Tree</td>
                <td>74.8%</td>
                <td>75.3%</td>
            </tr>
            <tr>
                <td>With SMOTE</td>
                <td>Random Forest</td>
                <td>84.3%</td>
                <td>83.9%</td>
            </tr>
        </table>

        <div class="key-insight">
            <strong>Key Insight:</strong> Random Forest Classifier performed best with 84.3% accuracy and 83.9% F1-score after balancing the dataset.
        </div>

        <h3>Skills & Tools</h3>
        <ul>
            <li><strong>Libraries:</strong> Pandas, Seaborn, Matplotlib, Scikit-learn, Imbalanced-learn</li>
            <li><strong>Techniques:</strong> Data scaling (StandardScaler), feature engineering, balancing class distribution (undersampling, SMOTE)</li>
        </ul>
    </section>

    <section>
        <h2>Project 2: Credit Card Fraud Detection</h2>
        <h3>Objective</h3>
        <p>Detect fraudulent transactions in a highly imbalanced credit card dataset while improving key evaluation metrics like precision, recall, and F1-score.</p>

        <h3>Challenges</h3>
        <ul>
            <li>Highly imbalanced data: ~99.8% transactions are normal, while ~0.2% are fraudulent.</li>
            <li>Maintaining high recall and F1-score without compromising precision.</li>
        </ul>

        <h3>Key Steps and Techniques</h3>
        <ul>
            <li><strong>Data Preprocessing:</strong>
                <ul>
                    <li>Normalized the Amount column using StandardScaler.</li>
                    <li>Removed the Time column as it was not relevant for modeling.</li>
                    <li>Handled duplicate data to reduce redundancy.</li>
                </ul>
            </li>
            <li><strong>Class Imbalance Management:</strong>
                <ul>
                    <li>Undersampling: Reduced majority class to match the minority class (473 samples each).</li>
                    <li>Oversampling: Methods like SMOTE can be applied for better results.</li>
                </ul>
            </li>
        </ul>

        <h3>Performance Results</h3>
        <table>
            <tr>
                <th>Algorithm</th>
                <th>Accuracy</th>
                <th>Precision</th>
                <th>Recall</th>
                <th>F1-Score</th>
            </tr>
            <tr>
                <td>Random Forest</td>
                <td>99.95%</td>
                <td>90.7%</td>
                <td>74.7%</td>
                <td>81.9%</td>
            </tr>
        </table>

        <div class="key-insight">
            <strong>Key Insight:</strong> Successfully addressed the data imbalance issue and demonstrated the importance of metrics like precision, recall, and F1-score over accuracy in imbalanced datasets.
        </div>

        <h3>Future Steps</h3>
        <ul>
            <li>Implement oversampling techniques like SMOTE to enhance recall and precision.</li>
            <li>Perform hyperparameter tuning for improved performance.</li>
        </ul>
    </section>

</body>
</html>

