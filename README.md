# Diabetes_Prediction_ML
I test various models to test which is the best for predicting diabetes for the given dataset (Patient is diabetic or not).

I extracted the 2 datasets from another github repo. (forgot it's name), they are in the "datasets" folder. In my code, I combined them as they are basically different features for the same patients.
I have gone through much detail to explain all the steps I have taken in the notebook itself.

I have used 2 approaches -

  1. The dataset is imbalanced, I didn't balance it for approach 1 and used Logit Model to calculate statistically relevant features
  2. I balanced the dataset, and then used RFE (using Logistic Regression) instead of Logit model as it performed relatively better.

I compared every result provided by each approach. I applied RandomForest, ADABoost, DecisionTrees, NaiveBayes, MLP and SVM.


Here are the comparisons :

# Approach 1

Precision Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Unbalanced%20Precision.png?raw=true)

Recall Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Unbalanced%20Recall.png?raw=true)

F1 Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Unbalanced%20F1.png?raw=true)

Accuracy Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Unbalanced%20Accuracies.png?raw=true)

# Approach 2

Precision Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Balanced%20Precision.png?raw=true)

Recall Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Balanced%20Recall.png?raw=true)

F1 Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Balanced%20F1.png?raw=true)

Accuracy Scores:
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Balanced%20Accuracies.png?raw=true)



Cross Validation Scores (Approach 2) :
![alt text](https://github.com/GaganMalik025/Diabetes_Prediction_ML/blob/main/Comparisons/Balanced%20CVs.png?raw=true)


In the end, I attained ~90% accuracy by RandomForest in Approach 2.
