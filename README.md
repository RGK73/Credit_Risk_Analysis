# Credit_Risk_Analysis
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, analyze, predict credit risk.

Overview of the loan prediction risk analysis:

Background:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. We used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.Various libraries and algorithms were used to build and evaluate models using resampling including:

imbalanced-learn
scikit-learn
RandomOverSampler
SMOTE algorithms
ClusterCentroids algorithm
SMOTEENN algorithm
BalancedRandomForestClassifier (bias reduction model)
EasyEnsembleClassifier (bias reduction model)

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once we’re done, we’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

Purpose of this analysis:
Explain how a machine learning algorithm is used in data analytics.
Create training and test groups from a given data set.
Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
Compare the advantages and disadvantages of each supervised learning algorithm.
Determine which supervised learning algorithm is best used for a given data set or scenario.
Use ensemble and resampling techniques to improve model performance.

Results:
The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:

Naive Random Oversampling
![alt_text]()Pic 1

Balanced Accuracy: 0.6612700484668286
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .66/.67
SMOTE Oversampling
![alt_text]()Pic 2

Balanced Accuracy: 0.6303296388959394
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .62/.64
Undersampling
![alt_text]()Pic 3

Balanced Accuracy: 0.6303296388959394
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .63/.40
Combination Under-Over Sampling
![alt_text]()Pic 4

Balanced Accuracy: 0.5173713090878325
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .70/.57
Balanced Random Forest Classifier
![alt_text]()Pic 5

Balanced Accuracy: 0.7877672625306695
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .67/.91
Easy Ensemble AdaBoost Classifier
![alt_text]()Pic 6

Balanced Accuracy: 0.925427358175101
Precision: The precision is low for High-risk loans and is high for Low-risk loans.
Recall: High/Low risk = .91/.94
Summary:
When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy. The other models were below .80 balanced accuracy. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.
