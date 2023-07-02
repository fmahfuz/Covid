
# Predicting death of COVID patient 

The main goal of this project is to build a data science tecniques that, given a Covid-19 patient's current symptom, status, and medical history, will predict whether the patient is in high risk or not.

## Dataset
The dataset was provided by the Mexican government. This dataset contains an enormous number of anonymized patient-related information including pre-conditions. The raw dataset consists of 21 unique features and 1,048,576 unique patients.
## Data Cleaning
Out of the 21 features only the columns ICU, INTUBED and PREGNANT has considerably large amount of missing data. For this reason the columns ICU and INTUBED, was dropped from the dataset. All missing values for PREGNANT are for males who can not be pregnant. So tha was replaced the missing value with 2 (which represents not pregnant). 
## Exploratory Data Analysis
I created a correlation plot to see how strongly related the features are with my target variable (DEATH column) 

Then I looked into the features in depth that are strongly correlated to the target variable. I began by plotting age and gender of the patient and observed elderly male patient are high risk.

## Model selection
For my model I chose Random Forest classifier, Naive Baise, Gradient Boosting classifier and k-nearest neighbor classifier and focused on the model with highest accuracy.
Out of the four models Random Forest Classifier performed the best with high accuracy (93.75%) and low false negative.