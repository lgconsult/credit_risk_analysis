# credit_risk_analysis

## Overview
The purpose of this analysis is to train a machine learning program to accurately assess credit risk of lending customers. We applied six different learning models to understand which one might work better. The models included oversampling, SMOTE oversampling, undersampling, combination over and under sampling, random forest classifier, and easy ensemble AdaBoost classifier.
  
## Results
### Oversampling
The balanced accuracy score for oversampling was .65 meaning that this model was only accurate at making predictions 65% of the time.
The precision for high risk lenders was .01, while the precision for low riks lenders was 1.0. This means that the model was not predicting high risk lenders accurately
The recall score for high risk lenders was .61, while for low risk lenders it was .68. This means that the model had a higher chance of predicting that a lender was low rick rather than high risk.
This model should probably not be used because it seems to default most as low risk and missing many high risk applicants. A model that overcorrects for high risk might be more desirable because false positives would be easier to fix via customer service.


### SMOTE oversampling
The SMOTE oversampling method left us with a balanced accuracy score of .62, meaning this model was accurate at making predictions 62% of the time, less than the previous oversampling method.
The precision for high risk borrowers was again .01 and low risk was again 1. This again means that the model had a higher chance of predicting that a borrower was high risk inaccurately
The recall score for high risk lenders was .61 and for low risk was .64, meaning that the model again had a higher chance of predicting that a lender was low risk rather than high risk.
This model is even less accurate than the previous, we should keep exploring other methods.

### Undersampling
 The undersampling method left us with a balanced accuracy score of .51, significantly lower than the previous two models.
 The precision score was again .01 for high risk and 1 for low risk borrowers. This model again failed to accurately predict high risk borrowers.
 The recall score was .57 for high risk and .45 for low risk. This means that those who are high risk only had a 57% chance of being marked high risk by the model, not a great statistic again.
 
 ### Combination over and under sampling
 The undersampling balanced accuracy score was 64%, meaning this model was accurate 64% of the time.
 The precision score was again .01 for high risk and 1 for low risk, meaning this model has a high probability of producting false negatives.
 The recall score was .7 and .58 for high risk and low risk borrowers respectively, meaning this model would produce false positives 30% of the time. This is a better model than any of the previous because false positives would be easier to clear up than false negatives.
 
 
### Random Forest Classifier
The random forrest classifier had balanced accuracy score of .66, meaning it was accurate 66% of the time.
The precision score for high risk borrowers was .74 and for low risk was 1, meaning this model would certainly produce a significant number of false negatives.
The recall score is .32 for high risk and 1 for low risk, meaning this model would produce false positives 68% of the time.
This model is better than the first three but not better than undersampling.

### Easy Ensemble AdaBooster Classifier
The random easy ensemble AdaBooster classifier had a balanced accuracy score of .85, significantly higher than all other methods.
The precision score for high risk borrowers was .89 and for low risk was .81, meaning this model only has a 19% chance of producing false negatives.
The recall score for high risk borrowers was .81 and for low risk .89 meaning this model again has a 19% chance of producing false positives.
balanced accuracy score

## Summary
The easy ensemble adabooster classifier is easily the best model to use in this analysis. It has the lowest likelihood of producing false negatives, which would be difficult to correct when approving borrowers for new lending. It also had the lowest chance of producing false negatives, which would be easier corrections to make. The other models all performed about the same in that they had a 100% chance of producing false negatives and should not be used for this analysis.
precision and recall scores
