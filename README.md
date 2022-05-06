
# Capstone Project Title
Employee Attrition Analytics

## Objectives

There are three main objectives for this analysis.

• Identify factors influencing attrition

• Predict possible attritions

• Identify possible ways to retain high performers

## Steps used:
Feature EXtraction using WOE scores
Cluster Analysis

## Model Development:
Build 2 models on
 Regularized Logistic Regression(C=10, class_weight='balanced', penalty='l1', random_state=42,solver='liblinear')
Decision trees: Default parameters

## Model Evaluation:
We have selected AUC ROC Curve & f1 score  as the evaluation criteria.
Optimal Cutoff - Using Youdens J statistic & Precision_Recall curve - 0.782603

## Best Model:
Logistic Regression model is selected because
It has high roc_auc_score than Decision Tree
comparable F1 score percentage and low standard deviation than Decision Tree
Logistic Regression has high recall (0.98) than Decision Tree (0.93)


## Factors Preventing Attrition:

Total_Available_Hours
Total_Training_Hours
Total_Leave_Hours
Supervisor_change_Yes
Position_Promoted_Yes
category_Confirmed Staff
category_Fixed term Staff
category_Serving Notice Period
category_Staff on Probation
category_Secondee-Outward-Without Pay

## Factors Affecting attrition

Profit Centre - 5
Profit Centre - 6
Location 7
Location 2
Supervisor Grade

## Performance on test data
** Cross validation results on TEST DATASET:**
Mean roc_auc_score Percentage for TEST dataset is: 98.487
Mean f1_scores Percentage for TEST dataset is: 84.81 

## Model Interpretation 
* Profit center 6 and 5 are positive variables, hence HR needs to look at what is happening in these location/center that is having a negative impact on the employee retention.
* Inspect what is happening on Location 7 and 2 
* Profit center 3 and 4 are negative variables, hence HR needs to look at what is happening in these location/center that is having a positive impact on the employee retention.
* Total Training hours , Total leave Hours , Total available hours  are variables of interest, need to be ascertained as to why employees with better training are staying, and why are employees with less training hours prone to leaving.
* Staff on probation, confirmed , secondee, on notice period and fixed staff are staying, if taken care of by providing adequate training and growth opportunities.
* Supervisor_Grade have a role in attrition and those under danger category had to be given proper training
* Employees who are Promoted are likely to stay

## Recommendations:

* Focus on Employee Training
* Feeling of job security prevents attrition.
* Mapping right set of employee to Right profile/profit center.
* Employee welfare w.r.t leaves, Total work hours to be monitored.

## Retention Measures

* Reason for Leaving- Reason for Leaving
Career growth is highest reason followed by personal and further studies 
Males are citing career growth as the major reason.

* New hires from syllible are churning more than any.
* Time to Hire - More termination happened during september.
So it’s better to hire before September.

* Supervisor - Under - and Hedi most number of resignation happened
More Personal issues with supervisors  “_” and “Terza Gwyn”
Employees under  “Lindy marguerite”  & “Hedi Elna” are concerned with career growth.
