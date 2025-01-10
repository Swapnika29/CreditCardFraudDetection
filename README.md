# CreditCardFraudDetection
## Research question:

### Which model will be best suited for classification of credit card fraud transactions?
 
Our task can be considered a supervised learning classification problem since we 
must predict transactions as Fraudulent or Non-Fraudulent. Correct classification of 
transactions is important so that accurate model training. However, without this 
labelling, the model would not be able to distinguish between these two transaction 
types and thus it would fail in real time. Classification can be used to check 
performance of the model through different metrics like accuracy, precision, recall, 
F1-score.

## Dataset:
Dataset was obtained from Kaggle (Credit Card Transactions Fraud Detection Dataset (Kaggle. com)). The dataset is a tabular with transactions occurred in 
September 2013 by European cardholders and provided by a collaboration between Worldline and the Machine Learning Group at Université Libre de Bruxelles. It includes 284,807 transactions over two days, with 492 frauds, highlighting a real world scenario. The dataset has V1 to V28 variables which are generated after PCA 
is not revealed due to privacy© issues.

## Why this dataset?
The reasons I chose this dataset:

Developing model on this dataset improves the relevant skills required to work in FinanicialTech industry. Credit card fraud is getting increase now a days due to the increase in digital transactions. There is an urgency for effective anti-fraud systems now more than ever. So, the need to have professionals in such areas is most acutely felt. The dataset offers many interesting technical challenges useful for practicing and improving upon more advanced data science and machine learning skills, such as handling very imbalanced data or using features that have been anonymized.

## Algorithms that will be used:
I am going to use several machine learning algorithms in order to test their effectiveness of detecting fraudulent transactions from the following: Support vector 
machine (SVM), Decision tree classifier, Logistic Regression, K- Nearest Neighbors(KNN).

Support Vector Machine (SVM): Since SVM works well with high dimensional spaces and is capable of modelling non-linear data separation using kernel tricks, I 
chose this as my model.

Decision Tree: I have chosen this because of its interpretability and super easy use in binary classification.

Logistic Regression: Chosen as it is fast and simple for binary classification problems.

K-Nearest Neighbors (KNN): Reliable since it is easy to understand and implement, a powerful classification method; in this algorithm samples would be classified based on its nearest points.

## Preprocessing:
There are no Missing Values in the dataset implying we do not have to handle missing data. The dataset contains an extremely imbalanced dataset therefore, I will 
take care of it in the modelling by deploying techniques (SMOTE for example) to make a more balanced dataset. Feature transformation was performed over the 28 
features which are anonymized excluding time and amount, such that confidential data is not revealed (Taken from original file). Apart from it, I plan to use 
StandardScaler() method on ‘Amount’ feature so that the distribution of data for this particular column will get normalised and also model performance become better.

## Performance Metrics:
The performance will be measured using following metrics:

Accuracy: It tells us the degree to which data is correct.

Precision: It tells us whether transactions that are marked as fraudulent, actually are.

Recall: It tells the model how many of all actual fraudulent transactions were flagged as fraudulent by the model.

F1-Score: F1 Score is the weighted average of Precision and Recall.

Confusion matrix: A table used to describe the performance of a classification model. It includes True Positives, True Negatives, False Positives and False 
Negatives.

## Purpose:
The main goal is to deploy a variety of machine learning models that correctly identify fraudulent transactions in an imbalanced dataset. On the other end, one of 
my goals in this project is to use a technique called Synthetic Minority Over-sampling Technique (SMOTE) to overcome some difficulties regarding imbalance and thereby increase model sensitivity. Finally, we will evaluate the performances of models using accuracy as performance metric and look at other metrics like precision, recall (sensitivity) or F1-score to understand which model suits best for real-time fraud detection system.

Building such a predictive model which can predict fraud transaction in real time would help avoid financial losses for cardholders and issuer companies, increasing to the bank's customers
