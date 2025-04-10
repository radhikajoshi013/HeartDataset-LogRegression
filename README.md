# HeartDataset-LogRegression

Problem Statement: Using Logistic Regression to find factors causing heart diseases

Data: Heart Disease Dataset (https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

Data Mining Operations: Log regression used with scikit-learn libraries (sklearn.model_selection, sklearn.preprocessing, sklearn.linear_model, sklearn.metrics)

Model Outputs: Pairplots, ROC Curve, feature importance from log regression.

Limitations: Challenges in selection of features for better model performance.

Results: Accuracy scores, confusion matrix and classification report were used to analyze performance. Dropping Fasting Blood Sugar (fbs) and Resting Electrocardiographic Results (restecg) column since they have low correlation with target, resulted in better performance.

