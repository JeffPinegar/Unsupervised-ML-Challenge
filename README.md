
# Jeff Pinegar
jeffpinegar1@gmail.com<br>
717-982-0516

# Unsupervised-ML-Challenge
Challenge 20 Unsupervised Machine Learning Challenge<br>
In this assignment, you will be building a machine learning model that attempts to predict if a person has Myopic vision or not.

## Summary

Whenever we have attempted to analyze the Myopia data, no Machine Learning model has ever been useful at predicting or classifying myopia.  In this attempt, we used Principle Component Analysis in an attempt to reduce the number of variables in the model while retaining much of the variation.  The principal components are also orthogonal.   With this data set to retain 90% of the variation, we needed 10 principal components, nearly equal to the 14 variables we started with. However, the 10 PC are orthogonal so they should yield a model with higher accuracy, at the expense of interpretability.

## Three Attempted Models
In an effort to construct a good model I actually made three attempts.
* JSP_Unsupervised_ML.ipynb – this model follows the direction for the assignment and starter code.
* JSP_Unsup_ML Drop Corr.ipynb  -- Upon inspection, the data set contains 4 variables with perfect correlation.  So I redid the assignment with 3 of those variables dropped.
* JSP_Unsup_ML drop corr and PCA.ipynb  -- With the three variable dropped, the PCA still require 9 components to account for >90% of the variance, and there are only 11 variables.  Therefore I redid the assignment again without PCA.

## Results

1. JSP_Unsupervised_ML.ipynb ---- precision =  0.1169 ---- accuracy =  0.4660<br>
2. JSP_Unsup_ML Drop Corr.ipynb  ---- precision =  0.1522 ---- accuracy =  0.7136 <br>
3. JSP_Unsup_ML drop corr and PCA.ipynb ---- precision =  0.1583  ---- accuracy =  0.7152.<br> 

## Conclusions
* Cleaning the data has the biggest impact.  The model improved by removeing the correlated variables.  Model 2 is much better then #1.
* Pincipal component Analysis (PCA) did not improve the results.  Model 3 is better than Model 2.  In addition model 2 is eaiser to understand.
* Non of thes model are very good.  Model 3 is the best, here are all the scores for this model:
  *  True positives (TP): 22
  * True negatives (TN): 420
  * False positives (FP): 117
  * False negatives (FN): 59
  * precision =  0.1583
  * accuracy =  0.7152
  * sensitivity =  0.2716  
