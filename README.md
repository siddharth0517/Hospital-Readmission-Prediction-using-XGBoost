# Hospital Readmission Prediction using XGBoost
## Project Overview
This project aims to predict hospital readmission rates based on patient data using the **XGBoost** machine learning algorithm. By leveraging a dataset with various patient metrics and medical details, this model can help in identifying high-risk patients and reduce hospital readmission rates.

## Dataset
The dataset consists of 25,000 records with 17 columns representing features such as patient age, the time spent in the hospital, the number of procedures, medications, and diagnoses, among others.
Download Dataset from this [LINK](https://www.kaggle.com/datasets/dubradave/hospital-readmissions)

## Key Features:
+ age: Age group of the patient (converted to a numeric range)
+ time_in_hospital: Number of days the patient spent in the hospital
+ n_procedures: Number of procedures performed on the patient
+ n_medications: Number of medications prescribed
+ n_outpatient, n_inpatient, n_emergency: Counts of outpatient, inpatient, and emergency visits
+ medical_specialty: The medical specialty of the doctor (one-hot encoded)
+ diagnosis codes (diag_1, diag_2, diag_3): Primary, secondary, and tertiary diagnoses (simplified and one-hot encoded)

## Target:
+ readmitted: Whether the patient was readmitted within a certain period (binary classification: Yes/No)

## Preprocessing
+ Handling Missing Data: Missing values in the medical_specialty column were imputed with the most frequent category.
+ Categorical Encoding: The age group was converted into numeric values, and categorical features such as medical_specialty and diagnosis codes were one-hot encoded.

## Model
The XGBoost classifier was used for training and predicting hospital readmissions.

## Evaluation Metric: Accuracy and cross-validation score
![image](https://github.com/user-attachments/assets/cba68b1d-823a-42b1-a5fd-1a70ee843cfc)

## Model Performance
After training the model and performing K-Fold cross-validation (with k=10), we achieved an overall accuracy of **92%** in predicting whether a patient will be readmitted.

## Conclusion
The model demonstrated a high predictive accuracy of **92%**, making it a promising tool for identifying patients at risk of hospital readmission. Future work could involve feature engineering and hyperparameter tuning to further improve the model's performance.

## Author
Siddharth Jaiswal

