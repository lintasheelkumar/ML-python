Credit card fraud happens when consumers give their credit card number to unfamiliar individuals,
 when cards are lost or stolen, when mail is diverted from the intended recipient and taken by criminals, 
or when employees of a business copy the cards or card numbers of a cardholder. 
In this notebook we will develop a few ML models using anonymized credit card transaction data. 
The challenge behind fraud detection is that frauds are far less common as compared to legal transactions



This dataset is severely imbalanced (most of the transactions are non-fraud).
 So the algorithms are much more likely to classify new observations to the majority class and high accuracy won't tell us anything. To address the problem of imbalanced dataset we can use undersampling and oversampling data approach techniques. Oversampling increases the number of minority class members in the training set. The advantage of oversampling is that no information from the original training set is lost unlike in undersampling, as all observations from the minority and majority classes are kept. On the other hand, it is prone to overfitting. There is a type of oversampling called SMOTE (Synthetic Minority Oversampling Technique), which we are going to use to make our dataset balanced. 
It creates synthetic points from the minority class

Also we shouldn't use accuracy score as a metric with imbalanced datasets (will be usually high and misleading), instead we should use f1-score, precision/recall score and confusion matrix

Recall of fraud cases (sensitivity) summarizes true positive rate (True positive/True positive + False Negative) - how many cases we got correct out of all the positive ones
Recall of non-fraud (specificity) summarizes true negative rate (True negative/True negative + False positive) - how many cases we got correct out of all the negative ones
Precision of fraud cases (True positive/True positive + False positive) summarizes the accuracy of fraud cases detected - out of all predicted as fraud, how many are correct
Precision of non-fraud cases (True negative/True negative + False negative) summarizes the accuracy of non-fraud cases detected - out of all predicted as non-fraud, how many are correct
F1-score is the harmonic mean of recall and precision
