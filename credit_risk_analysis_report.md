# Credit Risk Modelling

## Overview of the Analysis

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

### The purpose of this report is to analyse the credit experience of the 'Company' and in particular use certain
### methodolgies to predict the likelihood that a loan would become impaired. It should be noted that aiming for 
### 100% sound loans would mean extremely strict loan conditions and would likely severly limit the amount of business
### the company could do. 

### We have used a range of available data that we believe is indicative of the quality of loans. We
### alse note that the credit policy may have changed over the past years in line with the state of the economy.

### We have used data on 77,536 loans of which just over 3% have become impaired. For each of the loans we have
### used the loan size, interest rate, the borrowers income, loan size and debt ratios together with some
### behavioural factors.

### we have used a 'Logistic Regression Model' to predict which loan may become impaired and analysed the
### predictive quality produced using standard metrics. Because the number of impaired loans is only 3%  
### the correct predictions of impairement was felt to be unsafe, we then used a technique to notionally 
### rebalance the loan population. The results suggest that the modified model can identify likely 
### impairement with over 85% probability. The data was split between 'Training Data" and 'Testing Data'
### to ensure the model performed well on loans that it was not trained on 

## Results of the Analysis based on the 'test data'

* Logistic Regression Model: 
  * Accuracy: 97% of the time correctly predicted unimpaired loans but only 4% of impaired loans  
  * The precision and recall metrics performed simiarly to the accuracy



* Logistic Regression Model with resampled training data:
  * Accuracy: 100% of the time correctly predicted unimpaired loans and 84% of impaired loans
  * The precision and recall metrics performed simiarly to the accuracy

### Recomendation

## We strongly recommend using the Logistic Regression Model with resampled training data, since the 
## accuracy and precision are most satisfactory. We also recommend that you re-examine and rebuild
## the model on a regular basis or if there is a change of credit policy.