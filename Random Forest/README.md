# Ensemble Models: Random Forest (Predicting Bankruptcy in Taiwan)
This Jupyter notebook demonstrates the Random Forest modeling of the Taiwan bankruptcy data.The goal of the model is to predict the target variable based on the input features.And my target variable is the "bankrupt" variable.


# Data Preparation
The first step in building the model is to split the data into training and testing sets using the train_test_split() function. The training set was used to train the model, while the testing set was used to evaluate its performance.

Since the data is imbalanced, with more samples in one class than the other, I used the oversampling technique. I resampled the training data using the OverSampler() method.


# Model Building
I extracted the cross-validation results from the model and loaded them into a DataFrame named cv_results. This allowed me to analyze the performance of the model and compare the results for different hyperparameters.

I extracted the best performing model and plotted a horizontal bar chart for the features that influenced the model. I also plotted a confusion matrix to evaluate the performance of the model on the testing data.


# Conclusion
In conclusion, I have built a random forest classifier model using oversampling and hyperparameter tuning with cross-validation. The model was evaluated using a confusion matrix and feature importance plot, which helped with the understanding of the performance of the model and identified the most important features.



