## The link of the dataset: "https://www.kaggle.com/mlg-ulb/creditcardfraud"

🛡️ Financial Sentinel: Ensemble ML for Fraud Detection

An in-depth analysis and model comparison study to identify the most robust and precise algorithm for detecting fraudulent credit card transactions in a highly imbalanced dataset.

📝 Table of Contents

About the Project

Key Findings & Best Model

Methodology & Models

Data Source

Getting Started

Dependencies

License

Contact

💡 About the Project

This project addresses the critical challenge of credit card fraud detection in finance. Given the highly skewed nature of real-world financial transaction data (where genuine transactions vastly outnumber fraudulent ones), selecting a model that prioritizes minimizing False Positives (Precision) is crucial to avoid incorrectly blocking legitimate customer transactions.

This analysis focuses on comparing the performance of six diverse models, using Python and Scikit-learn, to determine the optimal deployment candidate.

🏆 Key Findings & Best Model

The study compared six models across three key metrics: Accuracy, AUC-ROC Score, and Precision Score.

Best Model Recommendation

Model

Accuracy Score

AUC-ROC Score

Precision Score

Recommendation Rationale

Stacking Classifier (Recommended)

0.999544

0.924676

0.980198

Highest Precision, making it the most effective at minimizing costly false positives (blocking legitimate transactions). Recommended for deployment.

Random Forest

0.999579

0.958198

0.923729

Highest overall Accuracy and strong balance across all metrics, serving as a reliable alternative.

AdaBoost

0.999403

0.983902

0.857143

Highest AUC-ROC, indicating excellent class separation.

Conclusion Summary

The Stacking Classifier and Random Forest models stand out due to their high Precision and AUC-ROC scores. The Stacking Classifier is recommended as the best model overall for this dataset, as its superior precision directly translates to better customer experience and lower operational costs associated with false alarms.

🔬 Methodology & Models

The following machine learning algorithms were trained and evaluated on the imbalanced dataset:

DecisionTreeClassifier

ExtraTreeClassifier

RandomForestClassifier

GradientBoostingClassifier

AdaBoostClassifier

StackingClassifier (Meta-learning approach)

📚 Data Source

The analysis uses the publicly available, anonymized dataset of credit card transactions provided by ULB (Université Libre de Bruxelles).

Dataset: Credit Card Fraud Detection

Source: Kaggle

🚀 Getting Started

These instructions will help you run the analysis and reproduce the results on your local machine.

Dependencies

This project relies on standard data science libraries, which can be installed via pip:

pip install numpy pandas matplotlib seaborn scikit-learn


Running the Analysis

Clone the repository:

git clone [https://github.com/YourUsername/YourProjectName.git](https://github.com/YourUsername/YourProjectName.git)
cd YourProjectName


Download the data:
Obtain the creditcard.csv file from the source link and place it in the root directory.

Execute the Jupyter Notebook:
Open the Fraud_detectoripynb.ipynb notebook and run the cells sequentially to load the data, perform EDA, train the models, and generate the final comparison metrics.

🛠️ Dependencies

Library

Purpose

numpy / pandas

Data manipulation and storage

matplotlib / seaborn

Data visualization and plotting

sklearn

Machine learning models (Ensembles, Trees) and metrics
