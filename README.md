# Mobile Payment Fraud Detection using various ML classification Algorithm
This is a group project.

We are implementing Artificial Intelligence and Machine learning algorithm based fraud detection tools to predict Mobile payment fraud in this project. For this, we are using the synthetic Mobile Payments Dataset found in the Kaggle web site 
The input of the data to this algorithm is a mobile payment transaction and the output will be the transaction with the field isFraud set to ‘0’ (False) or ‘1’ (True) indicating whether the transaction is fraud or not fraud.

The data from this dataset is cleaned, transformed and perform SMOTE analysis / Random undersampling to handle imbalance. The upsampled or the undersampled data are used to train and validate the algorithms to predict if the transaction is fraud. Various ML technology Classification algorithms are used for the binary classification, to classify the Mobile payment transaction as fraud or non-fraud. 

We are using the below mentioned classification algorithms for this project. we are comparing the performance of the algorithms by predicting the fraud transactions.
•	Logistic regression

•	Random Forest Classifier

•	Gradient Boosting Classifier

•	AdaBoost Classifier

•	Support Vector Machines


The accuracy of the algorithms is evaluated using  following metrics such as Cross validation, Classification Accuracy, Confusion Matrix, Sensitivity, Specificity, Area under Curve (AUC)

Data Collection and Sources

The dataset can be found and downloaded from the link 
https://www.kaggle.com/ntnu-testimon/paysim1
This dataset has around 6.5 Million records out of which around 8500 are marked as fraud. The dataset is heavily imbalanced, So we have done upsampling of minority class in most of the algorithms, and downsampling of majority in SVM algorithm

The dataset has the following fields.

step – The step in the full transaction.
type – type of transaction. The dataset has 5 types of transactions.
amount – transaction amount
nameOrig – name of the person/organization who initiated the transaction. This is obfusticated.
oldbalanceOrg – Starting balance of the originator account.
newbalanceOrig – Ending balance of the originator after the transaction amount is posted.
nameDest – Name of the person/organization of the destination account.
oldbalanceDest – Starting balance of the destination account before the transaction amount is posted to the account
newbalanceDest – Ending balance of the destination account after posting the transaction amount.
isFraud –Boolean flag indicating if the transaction is fraud.
isFlaggedFraud – The description of this field is not clear. There are only 16 transactions out of 6 million that has a value of 1 in this field and rest are 0. 
