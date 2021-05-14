# Diabetes_Prediction_ML
I test various models to test which is the best for predicting diabetes for the given dataset (Patient is diabetic or not).

I extracted the 2 datasets from another github repo. (forgot it's name), they are in the "datasets" folder. In my code, I combined them as they are basically different features for the same patients.
I have gone through much detail to explain all the steps I have taken in the notebook itself.

I have used 2 approaches -

  1. The dataset is imbalanced, I didn't balance it for approach 1 and used Logit Model to calculate statistically relevant features
  2. I balanced the dataset, and then used RFE (using Logistic Regression) instead of Logit model as it performed relatively better.

I compared every result provided by each approach. I applied RandomForest, ADABoost, DecisionTrees, NaiveBayes, MLP and SVM.

In the end, I attained ~90% accuracy by RandomForest in approach 2.
