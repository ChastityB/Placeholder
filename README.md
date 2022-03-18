# Stroke Predictions Dataset

##Data Dictionary

Column Name | Data Type | Description
------------|-----------|------------
id | Integer | Unique identifier
gender | Object | "Male", "Female", "Other"
age | Float | Age of patient
hypertension |Integer | 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
heart Disease | Integer | 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
ever_married | Object | "No" or "Yes"
work_type | Object |  "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
Residence_type | Object | "Rural" or "Urban"
avg_glucose_level | Float | average glucose level in blood
bmi | Float | body mass index
smoking_status | Object | "formerly smoked", "never smoked", "smokes" or "Unknown"*
stroke | Integer | 1 if the patient had a stroke or 0 if not, target

*Note: "Unknown" in smoking_status means that the information is unavailable for this patient
