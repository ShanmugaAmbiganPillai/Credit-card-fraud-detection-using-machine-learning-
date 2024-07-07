Summary:
This dataset contains credit card transactions made by European cardholders in the year 2023. It comprises over 550,000 records, and the data has been anonymized to protect the cardholders' identities. The primary objective of this dataset is to facilitate the development of fraud detection algorithms and models to identify potentially fraudulent transactions.
This project will look at mainly 4 ML models : namely, Logistic, decision tree, random forest and neural network at detecting credit card fraud in our sample data set obtained on Kaggle
Problem Statement: Fraud can bring Financial loss to card members and financial institutes. The FTC( Federal trade Commission) had quoted that from the 5.1 million reports received in 2023, 46% of it were related fraud charges either on debit /credit  charge cards and the numbers has been increasing YoY till today. So we are looking at Building a model that  answers/solves our issue: reduce false positive because we only want to flag and filter out fraud charges and not legitamate charges. False positives can result in genuine transactions being flagged as fraudulent, leading to unnecessary declines of valid transactions. This can be frustrating for customers and may lead to customer dissatisfaction , thus by Ensuring a low false positive rate helps maintain customer loyalty.While preventing fraud is important, frequent false positives can lead to lost sales and reduced customer spending, impacting the financial performance of the institution.
Data cleaning: dropped empty colums that were null or not available and also removed the ID : column, which was just used to number the data set
Exploratory data analysis (EDA) I looked at corelation between the variables , z scores
Findings:
1.	Logistic Regression achieved an accuracy of ~96.49%.
2.	Decision Tree achieved an accuracy of ~99.93%.
3.	Random Forest achieved an accuracy of ~99.95%.
4.	Neural Network achieved an accuracy of ~99.94%.
1.	Logistic Regression False positive was  1270
2.	Decision Tree False positive was 180
3.	Random Forest False positive was 19
4.	Neural Network False positive was 232
Evaluation:•	Logistic Regression: High accuracy but may suffer from overfitting due to imbalance.
•	Decision Tree: Similar accuracy to Logistic Regression, interpretable but may overfit.
•	Random Forest: Best performance, robust to overfitting.
•	Neural Network: Good performance but requires more computational resources.
•	Logistic Regression: High accuracy but may suffer from overfitting due to imbalance.
•	Decision Tree: Similar accuracy to Logistic Regression, interpretable but may overfit.
•	Random Forest: Best performance, robust to overfitting.
•	Neural Network: Good performance but requires more computational resources.
Implementation:Integrate the model into the existing transaction processing system and picking up charges that are fraud upfront and notifying customers to confirm if charges are valid or fraud before taking necessary action of blocking card or keeping it active for usage.
