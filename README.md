# SyriaTel Classification Model

Author: Tai Ngoc Bui <br>
Date Completion: June 1st, 2024

## 1.Business Understanding
This project focuses on developing a robust and accurate predictive model to classify whether a customer will "soon" stop doing business with SyriaTel. This model should achieve a minimum prediction accuracy of 90% and recall rate of 80% for the churn class to ensure the model effectively identifies the most potential churners.

Besides building an effective model, this project also recommend the most important features to the SyrialTel team. These features will help stakeholders to implement targeted retention strategies to reduce customer attrition, thereby enhancing customer satisfaction and loyalty, and ultimately increasing revenue.


## 2.Data Understanding
This public dataset is provided by the Kaggle community's [Churn in Telecom's dataset](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset). It contains 20 predictor variables mostly about customer usage patterns. There are 3333 records in this dataset, out of which 483 customers are churners and the remaining 2850 are non-churners. Thus, the ratio of churners in this dataset is 14%. The data is clean overall with no duplicated row or Nan values.

Summary of Features in the Dataset

* state: the state the customer lives in
* account length: the number of days the customer has had an account
* area code: the area code of the customer
* phone number: the phone number of the customer
* international plan: true if the customer has the international plan, otherwise false
* voice mail plan: true if the customer has the voice mail plan, otherwise false
* number vmail messages: the number of voicemails the customer has sent
* total day minutes: total number of minutes the customer has been in calls during the day
* total day calls: total number of calls the user has done during the day
* total day charge: total amount of money the customer was charged by the Telecom company for calls during the day
* total eve minutes: total number of minutes the customer has been in calls during the evening
* total eve calls: total number of calls the customer has done during the evening
* total eve charge: total amount of money the customer was charged by the Telecom company for calls during the evening
* total night minutes: total number of minutes the customer has been in calls during the night
* total night calls: total number of calls the customer has done during the night
* total night charge: total amount of money the customer was charged by the Telecom company for calls during the night
* total intl minutes: total number of minutes the user has been in international calls
* total intl calls: total number of international calls the customer has done
* total intl charge: total amount of money the customer was charged by the Telecom company for international calls
* customer service calls: number of calls the customer has made to customer service
* churn: true if the customer terminated their contract, otherwise false

## 3. Objectives
* Develop a binary classification model to predict whether a customer will "soon" stop doing business with SyriaTel
* Explore and analyze to identify main features that would impact customers' decisions to stop using SyriaTel service
* Provide data-driven strategies to minimize the churning rate at SyriaTel.

## 5. Data Cleaning
This dataset has no Nan values and duplicated values. However, several features do have perfect correlations. Therefore, I decieded to drop several features which share perfect correlations to eliminate multicollinearity among the features.

![Corr Matrix](https://github.com/taingocbui/phase3_project/blob/main/photos/corr_matrix.png)

## 6. Preprocessing Process
Preprocessing process includes 3 steps:
* Process categorical features as a one-hot numeric array using scikit-learn library
* Splitting dataset after one-hot encoded into train and test set with test set's size is 25% of dataset
* As most features are normally distributed, they will be normalized with Standard Scaler so that each numerical feature will have mean = 0 and standard deviation = 1.

## 7. Logistic Regression


## 8. Decision Tree Classifier


## 9. Conclusion


## 8. Future Works
To better improve the quality of this report, I will extend this project using Random Forest Classifier model and Support Vector Machine model to possibly achieve a better accuracy and recall rate.

