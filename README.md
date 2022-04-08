# Stroke Predictions Dataset

## Summary
This dataset was imported, cleaned, and visualized. The purpose of this is to help create a model that can determine if a patient is likely to get a stroke based on the metabolic parameters provided.

## Data Dictionary

Column Name | Data Type | Description
------------|:-----------:|------------
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

## Data Cleaning
* Fixed inconsistency of values

## Data Visualization
* Created plots to determine what factors affected chances of stroke

## Machine Learning Model
* Median Imputer used for numerical values
* OneHotEncoded used for categorical values
* Data was scaled

## Model Comparison
* KNN Classifier
* Random Forest Classifier
* XGBooster

## Accuracy Comparisons
| | KNN Classifier| Random Forest Classifier | XGBooster
-------------|:---------------------------:|:----------:|:------:| 
Baseline - Training| 96%| 100%| 96%
Baseline - Testing| 94%|94%|96%
Hypertuned - Training| 96%| 96%|96%
Hypertuned - Testing| 94%|94%|94%


