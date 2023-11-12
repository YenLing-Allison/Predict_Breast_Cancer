# Predict_Breast_Cancer
https://github.com/YenLing-Allison/Predict_Breast_Cancer

# Business Question
1. Specifically, build a decision tree, logistic regression and k-nearest neighbors that predicts the diagnose result based on ten real-valued features (mean, standard error, and "worst" or largest of these features). Explore how well different model perform for several different parameter values. When is overfitting and when is underfitting? Show how you set the model that provides the best predictive performance.
2. Present a brief overview of your predictive modeling process, explorations, and discuss your results. Make sure you present information about the model “goodness” (possible things to think about: confusion matrix, predictive accuracy, classification error, precision, recall, f-measure).

# Data Resource
Dataset: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data  
Data description: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names

# Analysis Process
1. Split the data into Training, Validation, and Testing data
2. Build the models and tune hyperparameters
3. Plot the fitting graph to see when is underfitting and overfitting
4. Build the models using the best performance of validation data
5. Make a prediction
6. Evaluate performance
<img width="960" alt="analysis_process" src="https://github.com/YenLing-Allison/Predict_Breast_Cancer/assets/144725779/14f5e8b0-649e-4474-b0d1-55531875da80">


# Result
I use **f-measure** to compare different models, because f-measure combines the precision and recall score.
Besides f-measure, I use precision and recall sequently to evaluate models, because precision can give me information to capture actual Malignant/Benign among predictions of all Malignant/Benign.
According to different performance of different models, I think that **KNN is the best model**.
| Model | Accuracy |
| --- | --- |
| Decision Tree | 0.91 |
| Logistic Regression - L1 | 0.95 |
| Logistic Regression - L2 | 0.95 |
| KNN | 0.95 |

