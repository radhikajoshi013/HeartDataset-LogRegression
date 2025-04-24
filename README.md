# HeartDataset-LogRegression

## Code:
<a href="https://github.com/radhikajoshi013/HeartDataset-LogRegression/blob/main/Log_Regression.ipynb">
<code>Log_Regression.ipynb</code></a>

## Problem Statement: 
Using publically available heart disease dataset and conduct Logistic Regression on it to find major factors causing heart diseases.

## Data Source: 
Heart Disease Dataset from Kaggle: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset

Or use the attached csv file directly: <a href="https://github.com/radhikajoshi013/HeartDataset-LogRegression/blob/main/heart_dataset_for_log_regression.csv">
<code>heart_dataset_for_log_regression.csv</code></a>

## Data Modeling Steps: 
Log regression used with scikit-learn libraries (sklearn.model_selection, sklearn.preprocessing, sklearn.linear_model, sklearn.metrics)
<li>Data Description using Pandas</li>
<li>Exploratory Data Analysis using Pandas, Pairplots and boxplots
<img width="750" height="550" alt="image" src="https://github.com/user-attachments/assets/3362afe8-3716-4eb6-8b9b-fc5fd32708ae"/></li>
<li>Preprocessing: Finding nulls and duplicates</li>
<li>Print the correlation coefficient matrix <img width="750" alt="image" src="https://github.com/user-attachments/assets/a37ce1b1-19f3-460f-975f-b428f960b638"/></li>
<li>Normalize data using MinMaxScaler</li>
<li>Train the model (80-20 split) using Logarithmic Regression</li>
<li>Fit & Predict the Model</li>
<li>Model Evaluation using Accuracy Scores, Confusion Matrix and Classification Reports</li>
<li>Dropping further variables resulting in improved accuracy scores</li>

## Model Outputs: 
Confusion Matrix, ROC Curve, feature importance from log regression.

<img width="450" alt="image" src="https://github.com/user-attachments/assets/793c52fb-8285-4fe1-b91e-eee644e9a30b"/>
<img width="385" alt="image" src="https://github.com/user-attachments/assets/5ec08417-6cfc-4d84-aae6-ff01a626913f"/>
<img width="650" alt="image" src="https://github.com/user-attachments/assets/97bb5294-c720-4f4b-aa5e-147a4e3e8d85"/>


## Limitations:
Challenges in selection of features for better model performance.

## Results: 
Accuracy scores, confusion matrix and classification report were used to analyze performance. Dropping Fasting Blood Sugar (fbs) and Resting Electrocardiographic Results (restecg) column since they have low correlation with target, resulted in better performance.

