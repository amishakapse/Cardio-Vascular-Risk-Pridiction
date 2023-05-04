# Cardio-Vascular-Risk-Pridiction

## Introduction
Cardiovascular diseases (CVDs) are a group of disorders of the heart and blood vessels and include coronary heart disease, cerebrovascular disease, rheumatic heart disease and other conditions.High blood pressure, high blood cholesterol, and smoking are key risk factors for heart disease.There were more than 523.2 million cases of cardiovascular disease in 2019, an increase of 26.6% compared with 2010.

## Problem Statement
The data is from an ongoing cardiovascular study on residents of the town of framingham, Massachusetts. The classification goal is to predict whether the patient has a risk of 10 year coronary heart disease(CHD). The dataset provides the patient's information. It includes over 4000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic, behavoural, and medical risk factor.

## Insights
* Patients having high colestrol has 18% chance of risk than borderline(14%) and normal(10%)
* Patients having hypertension 25% chance of risk than prehypertension(14%) and normal(10%)
* Patients being Underweight and obese has 19% chances of risk than overweight(16%) and healthy(12%)
* Patients Having heart rate being normal and high has high chance than low.
* Patient being diabetic has 47% of chance of risk than prediabetic(17%) and normal(14%)
* Adult above 60 has high chance of risk.
* Patients smoking large number of cigrettes per day has high on risk
## Variables Description
### Demographic:
* Sex: male or female ("M" or "F")
* Age: Age of the patient (Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)
* Education: The level of education of the patient (categorical values - 1,2,3,4)
### Behavioral:
* is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes)
### Medical (history):
* BP Meds: whether or not the patient was on blood pressure medication (Nominal)
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
* Diabetes: whether or not the patient had diabetes (Nominal)
### Medical (current):
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)
* Glucose: glucose level (Continuous)
* Predict variable (desired target):
* 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”)

## Conclusion
### Conclusion From EDA
1.Age plays a significant role in determining the risk of CHD.

2.Men have a higher likelihood of developing CHD compared to women.

3.Smoking is a well-known risk factor for CHD, and the intensity of smoking further increases the risk.

4.Patients with high blood pressure, stroke, and diabetes are at an elevated risk of developing CHD.

5.Patients who have had a prevalent stroke or prevalent hypertension have a higher likelihood of being at risk for CHD.

6.Patients with diabetes have an increased risk of CHD.

7.Total cholesterol levels tend to be slightly higher in patients who are at risk for CHD.

8.There exists a positive association between certain variables such as age and systolic blood pressure, as well as between BMI and glucose levels, with the risk of CHD.

### Conclusion From Model Implementation
1.The Random Forest Classifier and XGBoost models outperformed the other four models tested in terms of accuracy, precision, and recall scores.

2.Although the KNN model had a relatively high recall score, its accuracy and precision scores were lower compared to those of the Random Forest Classifier and XGBoost models.

3.The SVC model had lower accuracy and ROC AUC scores, suggesting that it may not be the most suitable model for this specific classification problem.

4.The XGBoost model had slightly higher test accuracy and precision scores than the Random Forest Classifier, and a higher ROC AUC score, indicating that it may be a better choice for predicting cardiovascular risk.

5.Based on the presented results, the XGBoost model was chosen as the most suitable classification model for the cardiovascular risk prediction dataset, with an accuracy of 89.67%.
