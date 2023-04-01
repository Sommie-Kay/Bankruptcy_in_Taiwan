# Predicting Bankruptcy in Taiwan Using Decision Tree Model
This folder contains code and files related to implementing a decision tree on an imbalanced dataset. The dataset was split into training and test sets using random train test split. The code explores the dataset and uses resampling techniques to handle the imbalance in the data.


# Data Preprocessing
The dataset used in this project is an imbalanced dataset. The features of the dataset based on the target variable are symmetric, and the dataset also had multicollinearity, making it unsuitable for use with linear models. The data was explored to identify its features and characteristics before implementing the decision tree.To handle the imbalance in the dataset, both under and over sampling techniques were used. The accuracy score was compared for both techniques, and over sampling produced a better score.


# Evaluation
Finally, I evaluated the model's performance using a confusion matrix.The top 15 features that had the highest importance in the decision tree model were visualized