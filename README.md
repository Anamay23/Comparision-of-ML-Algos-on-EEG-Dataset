# Comparision-of-ML-Algos-on-EEG-Dataset

## Dataset and Work Done
This project focuses on the dataset collected from the Childern's Hospital Boston and consists of EEG recordings from pediatric subjects with intractable seizures. The [dataset](https://physionet.org/content/chbmit/1.0.0/) can be found here. The readings are then classified into 2 classes- seizure activity and non-seizure activity.
We look to apply different classification algorithms to predict whether the patient is showing seizure activity or not. Then after comparing the results, we look to apply hyperparameter tuning to one of the models to see if we can better its performance. Finally we end up evaluating the best performing model on the test data set and plotting an roc_auc_curve to show the results.

## Algorithms and Parameters Used
There have been a total of 6 classification models used to predict the output. They are:
1. K-Nearest Neighbors
2. Logistic Regression
3. Naive Bayes
4. Random Forest
5. Gradient Boosting
6. Decision Trees

We have also selected 6 parameters to evaluate each model on. They are:
1. Accuracy
2. Precision
3. Recall
4. F1-score
5. Specificity 
6. Matthews' Correlation Coefficient 

## Results and Conclusion
After evaluating the performance on training and validation sets, we see Random Forest, Gradient Boosting and Decision Trees as the models with high performance. We choose to perform hyperparameter tuning on the Decision Tree model to try and improve the performance but we see that the defaut values return the best performance. Now with Gradient Boosting as our best performing model, we evaluate it on our test data and plot an roc_auc_curve.

