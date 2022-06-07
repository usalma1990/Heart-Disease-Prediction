# Heart Disease Prediction

The goal of this machine learning model is to predict the binary class heart_disease_present, which represents whether or not a patient has heart disease:
•	0 represents no heart disease present
•	1 represents heart disease present


Dataset

There are 14 columns in the dataset, where the patient_id column is a unique and random identifier. The remaining 13 features are described below.
•	slope_of_peak_exercise_st_segment (type: int): the slope of the peak exercise ST segment, an electrocardiography read out indicating quality of blood flow to the heart
•	thal (type: categorical): results of thallium stress test measuring blood flow to the heart, with possible values normal, fixed_defect, reversible_defect
•	resting_blood_pressure (type: int): resting blood pressure
•	chest_pain_type (type: int): chest pain type (4 values)
•	num_major_vessels (type: int): number of major vessels (0-3) colored by flourosopy
•	fasting_blood_sugar_gt_120_mg_per_dl (type: binary): fasting blood sugar > 120 mg/dl
•	resting_ekg_results (type: int): resting electrocardiographic results (values 0,1,2)
•	serum_cholesterol_mg_per_dl (type: int): serum cholestoral in mg/dl
•	oldpeak_eq_st_depression (type: float): oldpeak = ST depression induced by exercise relative to rest, a measure of abnormality in electrocardiograms
•	sex (type: binary): 0: female, 1: male
•	age (type: int): age in years
•	max_heart_rate_achieved (type: int): maximum heart rate achieved (beats per minute)
•	exercise_induced_angina (type: binary): exercise-induced chest pain (0: False, 1: True)

Defining Variables

Here, the target variable is heart_disease_present. However, the remaining variables are the predictor variables 

Label Encoding 

Inorder to build a machine learning model, the categorical features will be encoded using label encoding 

Model Validation 

Using train test split, the data will be split into train and test in the ratio of 70 and 30 respectively 


Modelling

Random Forest Algorithm gives an accuracy of 83.3%

Hyperparameter tuning

Inorder to get better outcome, hyperparameter tuning is performed. Here, different values are set for random_state to check which value gives maximum accuracy. Here, random_state=0

Model Evaluation

The heart disease prediction model is evaluated based on accuracy. Here, crosstab has been used

