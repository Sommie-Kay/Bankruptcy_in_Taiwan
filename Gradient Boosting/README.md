# Predicting Bankruptcy in Taiwan Using Gradient Boosting Trees.
This notebook demonstrates the implementation of Gradient Boosting as an ensemble model to predict bankruptcy in the Taiwan bankruptcy dataset.Gradient boosting is a machine learning technique for building ensemble models by iteratively adding new weak learners to the ensemble while focusing on the samples that are difficult to classify correctly.


# Data Preparation
The first step in building the model is to split the data into training and testing sets using the train_test_split() function. The training set will be used to train the model, while the testing set will be used to evaluate its performance.

Since the data is imbalanced, with more samples in one class than the other, we used the oversampling technique. We resampled the training data using the OverSampler() method.


# Model Building
To build the model, we used the GradientBoostingClassifier() class from the sklearn.ensemble module. We trained the model using the oversampled training data.

Next, we performed cross-validation with the classifier, using the oversampled training data to tune hyperparameters and get the best performing model using GridSearchCV().


# Model Evaluation
I evaluated the performance of the model using a classification report, which provided precision, recall, F1-score, and support for each class. We also created an interactive dashboard that shows how the company's profit and losses change in relation to the model's probability threshold.

i created a function called make_cnf_matrix that calculated and printed profit/losses and displayed a confusion matrix. We also created a FloatSlider thresh_widget that ranges from 0 to 1. Finally, we combined the function and slider in the interact function.