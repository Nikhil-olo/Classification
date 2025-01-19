<h1>Classification</h1>

<h2>Project Summary: Credit Card Default Prediction</h2>
<p><b>Objective:</b> Developed a machine learning model to predict credit card default payment using the UCI Credit Card Default dataset with 30,000 samples and 24 features.</p>

<h3>Data Preprocessing & EDA</h3>
<h4>Exploratory Data Analysis (EDA):</h4>
<ul>
  <li>Analyzed correlations using heatmaps and visualized trends for key features like LIMIT_BAL, PAY_*, and AGE against default status.</li>
  <li>Used count, distribution, and box plots to understand data patterns.</li>
  <li>Identified and visualized class imbalance in the target variable (<i>default.payment.next.month</i>), with 78% non-defaults and 22% defaults.</li>
</ul>

<h4>Data Cleaning:</h4>
<ul>
  <li>No missing or duplicate values were detected.</li>
  <li>Removed irrelevant features such as ID for model optimization.</li>
  <li>Handled class imbalance through undersampling and SMOTE (oversampling).</li>
</ul>

<h3>Model Development & Evaluation</h3>
<h4>Algorithms Used:</h4>
<ul>
  <li>Logistic Regression</li>
  <li>Decision Tree Classifier</li>
  <li>Random Forest Classifier</li>
</ul>

<h4>Performance Metrics:</h4>
<ul>
  <li><b>Results with original imbalanced data:</b></li>
  <ul>
    <li>Logistic Regression: Accuracy: 81%, F1: 35.3%</li>
    <li>Random Forest: Accuracy: 81.2%, F1: 45.4%</li>
  </ul>
  <li><b>Results after undersampling:</b></li>
  <ul>
    <li>Logistic Regression: Accuracy: 66.4%, F1: 65.2%</li>
    <li>Random Forest: Accuracy: 68.8%, F1: 65.8%</li>
  </ul>
  <li><b>Results with SMOTE (optimal performance):</b></li>
  <ul>
    <li>Logistic Regression: Accuracy: 71.9%, F1: 71.9%</li>
    <li>Decision Tree: Accuracy: 74.8%, F1: 75.3%</li>
    <li>Random Forest: Accuracy: 84.3%, F1: 83.9%</li>
  </ul>
</ul>

<h4>Skills & Tools:</h4>
<ul>
  <li>Libraries: Pandas, Seaborn, Matplotlib, Scikit-learn, Imbalanced-learn</li>
  <li>Techniques: Data scaling (StandardScaler), feature engineering, balancing class distribution (undersampling, SMOTE)</li>
</ul>

<h4>Key Insights:</h4>
<ul>
  <li>Random Forest Classifier performed best with 84.3% accuracy and 83.9% F1-score after balancing the dataset.</li>
  <li>SMOTE improved model generalizability by addressing class imbalance effectively.</li>
</ul>

<h2>Project Summary: Credit Card Fraud Detection</h2>
<p><b>Objective:</b> Detect fraudulent transactions in a credit card dataset while improving key evaluation metrics like precision, recall, and F1-score.</p>

<h3>Key Steps and Techniques</h3>
<h4>Data Preprocessing:</h4>
<ul>
  <li>Normalized the <i>Amount</i> column using StandardScaler.</li>
  <li>Removed the <i>Time</i> column as it was not relevant for modeling.</li>
  <li>Handled duplicate data to reduce redundancy.</li>
</ul>

<h4>Class Imbalance Management:</h4>
<ul>
  <li>Undersampling: Reduced majority class to match the minority class (473 samples each).</li>
  <li>Oversampling: Used SMOTE for better results.</li>
</ul>

<h4>Machine Learning Models:</h4>
<ul>
  <li>Logistic Regression</li>
  <li>Decision Tree Classifier</li>
  <li>Random Forest Classifier</li>
</ul>

<h4>Performance Metrics:</h4>
<ul>
  <li>Random Forest Classifier performed best with:</li>
  <ul>
    <li>Accuracy: 99.95%</li>
    <li>Precision: 90.7%</li>
    <li>Recall: 74.7%</li>
    <li>F1-Score: 81.9%</li>
  </ul>
</ul>

<h4>Key Learnings:</h4>
<ul>
  <li>Successfully addressed the data imbalance issue.</li>
  <li>Highlighted the importance of metrics like precision, recall, and F1-score over accuracy in imbalanced datasets.</li>
</ul>

<h2>Project Summary: Email Spam Detection</h2>
<p><b>Objective:</b> Built a machine learning pipeline to classify email messages as spam or ham (non-spam).</p>

<h3>Key Steps and Techniques</h3>
<h4>Data Preprocessing:</h4>
<ul>
  <li>Verified dataset integrity: No missing or null values.</li>
  <li>Converted the <i>Category</i> column to binary format (spam: 0, ham: 1).</li>
  <li>Split the data into training and testing sets (80%-20% split).</li>
  <li>Used TfidfVectorizer with binary weighting to convert text data into feature vectors.</li>
</ul>

<h4>Machine Learning Models:</h4>
<ul>
  <li>Logistic Regression</li>
  <li>Decision Tree Classifier</li>
  <li>Random Forest Classifier</li>
</ul>

<h4>Model Performance:</h4>
<ul>
  <li><b>Logistic Regression:</b> Accuracy: 96.59%, F1 Score: 98.07%</li>
  <li><b>Decision Tree Classifier:</b> Accuracy: 96.77%, F1 Score: 98.15%</li>
  <li><b>Random Forest Classifier:</b> Accuracy: 97.76%, F1 Score: 98.72%</li>
</ul>

<h4>Key Learnings:</h4>
<ul>
  <li>Random Forest Classifier outperformed other models, achieving an F1 score of 98.72%.</li>
  <li>Demonstrated proficiency in working with text data using TfidfVectorizer, handling class imbalances, and evaluating multiple classifiers.</li>
</ul>
