# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk

## Overview of Challenge:   
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Different techniques were used to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, various libraries and algorithms were used to build and evaluate models using resampling including: 
* imbalanced-learn 
* scikit-learn
* RandomOverSampler
* SMOTE algorithms
* ClusterCentroids algorithm
* SMOTEENN algorithm
* BalancedRandomForestClassifier (bias reduction model)
* EasyEnsembleClassifier (bias reduction model)

## Purpose: 
1. Explain how a machine learning algorithm is used in data analytics.
2. Create training and test groups from a given data set.
3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
5. Compare the advantages and disadvantages of each supervised learning algorithm.
6. Determine which supervised learning algorithm is best used for a given data set or scenario.
7. Use ensemble and resampling techniques to improve model performance.

## Results:
I have listed the results for the learning models including their respective balanced accuracy, precision, and recall scores below:      

### Naive Random Oversampling
![Pic 1](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/RANDOM_oversampling.png)     
1. Balanced Accuracy: 0.643860465491054
2. Precision: The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .61/.68

### SMOTE Oversampling
![Pic 2](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/SMOTE_oversampling.png)     
1. Balanced Accuracy: 0.6521789928729992
2. Precision: The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .67/.64

### Undersampling
![Pic 3](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/UNDERSAMPLING.png)     
1. Balanced Accuracy: 0.6521789928729992
2. Precision:  The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .60/.42

### Combination Under-Over Sampling
![Pic 4](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/COMBO.png)     
1. Balanced Accuracy: 0.5107328039450306
2. Precision: The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .70/.58

### Balanced Random Forest Classifier
![Pic 5](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/Balanced_Learning.png)     
1. Balanced Accuracy: 0.7877672625306695
2. Precision: The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .67/.91

### Easy Ensemble AdaBoost Classifier
![Pic 6](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/AdaBoost.png)     
1. Balanced Accuracy: 0.925427358175101
2. Precision: The precision is **low** for High-risk loans and is **high** for Low-risk loans.
3. Recall: High/Low risk = .91/.94

### Summary of Models:
![Pic 7](https://github.com/mpournaras/Credit_Risk_Analysis/blob/main/resources/Summary.png)

## Summary:
When comparing balanced accuracy between models, I am looking for the closest number to 1 (between 0 and 1). For the credit data set provided, the Easy Ensamble AdaBoost Classifier model has a substantially higher balanced accuracy than the others at **.93**. Every other model's balanced accuracy fell below .78! The precision for all models was relatively similar but the AdaBoost still came out with higher precision at .07 for high risk and 1.0 for low risk. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The **Easy Ensemble AdaBoost Classifier** had the highest recall score as well, ultimately making it the best machine learning model to choose for further credit card analysis.

Completed by: Michael Pournaras
