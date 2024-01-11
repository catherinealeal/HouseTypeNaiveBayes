# House Type Classification Using Naive Bayes 

## Goal 

Use Naive Bayes to predict the house type of homes in Melbourne and compare the results of our classifier to skikit-learn's Naive Bayes classifier. 

## Data Loading and Preprocessing 

The date attribute is converted to a numeric value (seconds since epoch) in order to use it as a predicting variable in Naive Bayes. 

## Prior Probabilities 

The prior probability of each housing type is calculated and stored in a dictionary. 
- House: 0.452
- Duplex: 0.418
- Townhouse: 0.13

## Comparing Naive Bayes Classifications 

The Naive Bayes classification perfomed through my own written functions has an accuracy of %57. The classification performed by scikit-learn's GaussianBN() function first requires missing values to be imputed using the attributes' means. This classifier has an accuracy of only %37. 

Based on the fact that the accuracy decreased by 20% when using imputation for scikit-learn's classifier, I would say that the imputation process hurt the classifier. This could be because the mean values used to fill in missing values might not accurately represent that observation, causing it to be misclassified. 

## View full notebook [here](https://github.com/catherinealeal/HouseTypeNaiveBayes/blob/main/HouseTypeNaiveBayes.ipynb)
