# Predicting Bankruptcy in Taiwan

This repository contains code for a machine learning project that predicts bankruptcy in Taiwan using the Decision Tree model. The dataset used is highly imbalanced, with a majority of non-bankrupt companies and a minority of bankrupt companies. To deal with this, the data was oversampled using the SMOTE technique and ensemble models such as Gradient Boosting Trees and Random Forest modeling were used.The project also includes an interactive dashboard that shows how company profit and losses change in relationship to the model's probability threshold.


# Dataset

The dataset used in this project is the Bankruptcy Prediction dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Taiwanese+Bankruptcy+Prediction). The data was collected from 1999 to 2009. The goal is to predict whether a company will go bankrupt or not based on its financial ratios.


# Data Preprocessing

The initial data was in JSON format and compressed, so it was converted to a dictionary after decompression and then turned into a Pandas dataframe.Since the dataset was highly imbalanced, the SMOTE technique was used to oversample the minority class. This involves creating synthetic samples of the minority class to balance the dataset. The data was then split into training and testing sets for model training and evaluation.


# Model

The Decision Tree model was chosen for this project due to its ability to handle both categorical and continuous data, and its interpretability. Ensemble models such as Gradient Boosting Trees and Random Forest modeling were also utilized to improve model performance.


# Results

The Decision Tree model achieved an accuracy of 96.42% on the test set. The Gradient Boosting Trees and Random Forest modeling ensemble models achieved an accuracy of 94.66% and 97.64% respectively. The Random Forest ensemble model also had  a better precision and recall scores than the Decision Tree model.


# Files
**Working_with_json.ipynb**: This notebook shows the decompression and conversion process.

**Decision Tree**: This notebook contains the decision tree modelling process and the model saved as a pickle file.

**Random Forest**: This notebook shows the modeling and results with Random Forest and the model saved as a pickle file.

**Gradient Boosting**: This notebook shows the modeling and results with gradient boosting and the model saved as a pickle file.


# Conclusion

This project demonstrates the use of the Decision Tree model and ensemble models to predict bankruptcy in Taiwan using financial ratios. The results show that ensemble models can improve the performance of the model, particularly when dealing with imbalanced datasets. The code and dataset used in this project can be used as a basis for further research on bankruptcy prediction in other countries or industries.
