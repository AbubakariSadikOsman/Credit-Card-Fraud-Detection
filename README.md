# Credit-Card-Fraud-Detection
This project uses machine learning algorithms  to analyze and detect whether credit card is fraudulent or genuine. 

PROJECT TITLE: CREDIT CARD FRAUD DETECTION

1.	 The dataset includes credit card transactions performed in September 2013 by European cardholders. This dataset shows transactions that took place over     the course of two days, out of which there were 492 frauds out of 284,807 transactions. The dataset is quite uneven; frauds, which are in the positive     category, represent 0.172% of all transactions.
    The dataset contains only numeric input variables that have undergone PCA transformation. Unfortunately, we are unable to offer the original               characteristics and further context for the data due to confidentiality concerns. The major components derived from PCA are features V1, V2..., and         V28. The only features that have not been changed with PCA are "Time" and "Amount." The seconds that passed between each transaction and the dataset's     initial transaction are listed in the feature "Time." The transaction amount is represented by the feature "Amount," which may be utilized for example-     dependent, cost-sensitive learning. The response variable, feature "Class," has a value of 1 in cases of fraud and 0 in all other cases.

2.	 The machine-learning method used is supervised machine learning which uses correctly labeled data or independent variables (input/output) to predict       results (dependent variable). The supervised machine learning algorithm utilizes logistical regression for classification. The independent variables       (input to) are the transaction Amount, Time, and V1, ... V28. They are the predictors that are used to predict the dependent variable (output from),       ‘Class’ which is dichotomous or binary in nature (0 – genuine and 1 – fraudulent credit card).

3.	 Using Naïve Bayes as the benchmark for the machine learning algorithm I used in this project, which is logistic regression for classification, logistic     regression is supervised machine learning that uses independent variables to predict the dependent variable. The dependent is binary or dichotomous or     has two categories labeled “0” and “1.” High volume of data is favorable for logistic regression, unlike the Naïve Bayes method which does better           classification based due to small or fewer samples of data. Also, The features of the dataset are split in a linear fashion so if the features are         correlated, due to linear classification, logistic regression works more efficiently with data analysis and gives better results than Naïve Bayes.         Finally, logistic regression has a low bias and higher variance whiles Naïve Bayes has a higher bias and low variance.

4.	Strengths of Logistic Regression

   a.	In a low-dimensional dataset, logistic regression is less prone to overfitting.

   b.	Logistic regression is very efficient when the dataset has features that are linearly separable.

   c.	The outputs of a logistic regression are well-calibrated probabilities along with classification results.

   d.	Logistic regression has a low bias and higher variance.

Weaknesses of Logistic Regression
   
   a.	In high-dimensional datasets, logistic regression is prone to overfitting.

   b.	In linear regression, independent and dependent variables are linearly related. However, logistic regression requires that independent variables           are linearly related to the log odds (log(p/1-p)).

   c.	Logistic regression requires a large dataset and sufficient training for all the categories it needs to satisfy.

   d.	Logistic regression cannot solve non-linear problems since it has a linear decision surface.

5.		REPORT OF THE RESULTS
      After the exploration of the credit card dataset, it was evident that the dependent variable ‘Class’ has imbalanced values (0 and 1). It was               important      to balance those values before training the dataset for modeling. I employed both under-sampled and oversampled imbalance adjustment         techniques to          balance the dependent variable values.

      The classification accuracy of the model is 0.94 (94%) for both under-sampled and oversampled trained datasets. However, the misclassification rate         is 0.06 (6%). 

      The probability that the model’s true prediction was right (precision) is 0.92 (92%) and 0.96 (96%) for 0 (genuine credit cards) and 1 (fraudulent         credit cards) respectively.

      The model has a recall or sensitivity of 0.97 (97%) and 0.92 (92%) for 0 (genuine credit cards) and 1 (fraudulent credit cards) respectively.
   
      Finally, the model has an F1 score of 0.95 (95%) and 0.94 (94%) for 0 (genuine credit cards) and 1 (fraudulent credit cards) respectively.
