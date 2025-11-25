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
