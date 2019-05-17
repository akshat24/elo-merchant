# elo-merchant
Predicts the customer loyalty score for each card id based on a few million transactions for Elo. Dataset is sourced from Elo Merchant Recommendation Competion hosted on Kaggle.

Link for Dataset: https://www.kaggle.com/c/elo-merchant-category-recommendation/data

## Approaches tried:
1. Boosting 
2. Random Forests

## Objectives:
1. To offer performance (RMSE) similar to the full model by using as few variables as possible. 
2. Make the model more intepretable

For making the model interpretable and ensuring that the features are universally accurate and consistent, utilized <strong>SHAP</strong> scores for feature importance. 
<strong>SHAP</strong> scores are consistent across models and offer reliable feature selection, better than gain and split. 
(https://towardsdatascience.com/interpretable-machine-learning-with-xgboost-9ec80d148d27)

## RMSE:
1. Boosting with Hyptertuned Parameters (all variables): 3.686
2. Boosting with top 10 variables (tuned model): 3.703
3. Random Forest with all variables: 3.727
4. Random Forest with top 10 variables: 3.741
