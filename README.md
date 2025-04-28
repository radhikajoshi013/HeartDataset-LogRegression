# HeartDataset-LogRegression

## Code:
<a href="https://github.com/radhikajoshi013/HeartDataset-LogRegression/blob/main/Log_Regression.ipynb">
<code>Log_Regression.ipynb</code></a>

## Problem Statement: 
Using publically available heart disease dataset and conduct Logistic Regression on it to find major factors causing heart diseases.

## Data: 
Heart Disease Dataset from Kaggle: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset

Or use the attached csv file directly: <a href="https://github.com/radhikajoshi013/HeartDataset-LogRegression/blob/main/heart_dataset_for_log_regression.csv">
<code>heart_dataset_for_log_regression.csv</code></a>

The dataset contains following variables:
<li>Age: Age of the patient in years.</li>
<li>Sex: Gender of the patient (1 = male, 0 = female).</li>
<li>Cp (Chest Pain Type): Type of chest pain experienced (e.g., typical angina, atypical angina, non-
anginal pain, asymptomatic).</li>
<li>Trestbps (Resting Blood Pressure): Blood pressure in mm Hg measured at rest.</li>
<li>Chol (Serum Cholesterol): Cholesterol level in mg/dL.</li>
<li>Fbs (Fasting Blood Sugar): Whether fasting blood sugar is > 120 mg/dL (1 = true, 0 = false).</li>
<li>Restecg (Resting Electrocardiographic Results): Results of the resting ECG test (e.g., normal,
<li>ST-T wave abnormality, left ventricular hypertrophy).</li>
<li>Thalach (Maximum Heart Rate Achieved): The highest heart rate reached during exercise.</li>
<li>Exang (Exercise-Induced Angina): Whether angina was induced by exercise (1 = yes, 0 = no).</li>
<li>Oldpeak: ST depression induced by exercise relative to rest (measures heart stress).</li>
<li>Slope: Slope of the peak exercise ST segment (e.g., upsloping, flat, downsloping).</li>
<li>Ca (Number of Major Vessels Colored by Fluoroscopy): Number of major vessels (0-3) with
calcium deposits.</li>
<li>Thal (Thalassemia): Blood disorder type (e.g., normal, fixed defect, reversible defect).</li>
<li>Target: The presence or absence of heart disease (typically 1 = disease, 0 = no disease).
(NOTE: This is the target Variable)</li>


## Data Mining Operations: 
Log regression used with scikit-learn libraries (sklearn.model_selection, sklearn.preprocessing, sklearn.linear_model, sklearn.metrics) used to predict absence or presence of heart disease in the target variable (binary categorical variable).
<li>Data Description using Pandas</li>
<li>Exploratory Data Analysis using Pandas, Pairplots and boxplots
<img width="750" height="550" alt="image" src="https://github.com/user-attachments/assets/3362afe8-3716-4eb6-8b9b-fc5fd32708ae"/></li>
<li>Preprocessing: Finding nulls and duplicates</li>
<li>Print the correlation coefficient matrix <img width="750" alt="image" src="https://github.com/user-attachments/assets/a37ce1b1-19f3-460f-975f-b428f960b638"/></li>
<li>Normalize data using MinMaxScaler (sklearn.preprocessing)</li>
<li>Train the model (80-20 split) using Logarithmic Regression (sklearn.linear_model)</li>
<li>Fit & Predict the Model</li>
<li>Model Evaluation using Accuracy Scores, Confusion Matrix and Classification Reports (sklearn.metrics)</li>
<li>Dropping further variables resulting in improved accuracy scores</li>

## Model Outputs: 
Confusion Matrix shows decent True Positive and True Negative Rates, ROC Curve shows a high AUC of 0.94, feature importance from log regression shows the features of less importance that can be dropped to improve already high accuracy scores of 88%.

<img width="450" alt="image" src="https://github.com/user-attachments/assets/793c52fb-8285-4fe1-b91e-eee644e9a30b"/>
<img width="385" alt="image" src="https://github.com/user-attachments/assets/5ec08417-6cfc-4d84-aae6-ff01a626913f"/>
<img width="650" alt="image" src="https://github.com/user-attachments/assets/97bb5294-c720-4f4b-aa5e-147a4e3e8d85"/>


## Limitations:
Challenges in selection of features for better model performance due to lack of subject matter expertise. Can be rectified by contacting or collaborating with an SME.

## Results: 
Accuracy scores, confusion matrix and classification report were used to analyze performance. Dropping Fasting Blood Sugar (fbs) and Resting Electrocardiographic Results (restecg) column since they have low correlation with target, resulted in better performance.

