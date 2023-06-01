# Bank-Marketing-Effectiveness-Prediction-Classification-Project

# **Project Summary -**

1.	The given dataset is from direct marketing campaigns of a Portuguese banking institution. The campaigns were conducted by phone calls. The classification goal is to predict if the client will subscribe a term deposit or not.
2.	The following model were build such as Logistic Regression, Decision Tree,  K nearest Neighbour Classifier and Naive Bayes Algorithm and compared them using the evaluation metrics score.
3.	The project started with importing and understanding the dataset by observing the rows and columns, shape, info about the data types, statistical description about the numerical columns and counting the null values of each column.
4.	The null values  are checked  and replaced with suitable values and averages and made the columns ready for Exploratory Data Analysis.
5.	 EDA  performed by various Univarite, Bivariate and Multivariate analysis to get the idea of the dataset and to make necessary transformations and manipulations to be then used for data pre processing for modelling and also gain business insights from them.
6.	Some of the hypothesis test were performed and based on p values the decision of accepted/rejected the  null hypothesis. 
7.	In the feature engineering section feature manipulation was done  where some columns were dropped and missing values imputations were done. The outliers are handled by using Z score method. Categorical features are converted into  numerical features by using  One Hot encoding.
8.	For splitting the data the Train test split was used  and splitted the data into 80:20.The data imbalance was adjusted using SMOTE technique. Furthermore the scaling process of data was done. The important features were selected for modeling .After apply each model hyper parameter tuning was used to find best optimized parameters.
9.	 The following metric scores were used to  such as Confusion matrix, Accuracy, Precision, Recall, F1 Score ,Cohens Kappa Score and ROC-AUC Curve.
10.	The Logistic Regression model performs better than other models. The Proposed Logistic Regression model have the Accuracy: 81.6 %, Precision :83.86 %, Recall: 78.26 %, F1 Score : 80.96 %, Cohens Kappa Score : 63.2 % and Area Under Curve : 89.98 %. Which are more compared to aforementioned other models.
11.	It is concluded that proposed model is capable to predict the target variables using new dataset and the model will be used for business improvement in banking sectors. 

# **Problem Statement**

The dataset is associated to direct marketing campaigns of a Portuguese banking institution. The phone calls were used for marketing campaigns. Often, more than one contact to the same client was required, in order to assess if the product (bank term deposit) would be ('yes') or not ('no') subscribed. The classification goal is to predict if the client will subscribe to a term deposit (variable y).

### Variables Description 


### <b>Customers details: </b>
*   age (numeric)
*  job : type of job (categorical: admin, blue-collar, entrepreneur, housemaid,management, retired, self-employed, services, student, technician, unemployed, unknown)
*  marital : marital status (categorical: divorced, married, single, unknown; note: 'divorced' means divorced or widowed)
*  education (categorical:high.school, illiterate, professional.course, university.degree, unknown)
*  default: has credit in default? (categorical: no, yes, unknown)
*  housing: has housing loan? (categorical: no, yes, unknown)
*  loan: has personal loan? (categorical: no, yes, unknown)

### <b> Related with the last contact of the current campaign:</b>
*  contact: contact communication type (categorical: cellular,telephone)
*  month: last contact month of year (categorical: jan, feb, mar, april, may,june, july, aug, sep, oct, nov, dec)
*  duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration = 0 then y ='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

### <b>Other attributes: </b>
*  campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
*  pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
*  previous: number of contacts performed before this campaign and for this client (numeric)
*  poutcome: outcome of the previous marketing campaign (categorical: failure, nonexistent, success)


### <b>Output variable (desired target):</b>
*  y - has the client subscribed a term deposit? (binary: 'yes', 'no')

# **Conclusion**

**From EDA**


*   Most of the clients education are secondary and tertiary, and most clients job categories are blue color, management and technician. Most of the campaign carried out married customers only.
*   May,June, July months campaign are more and december, march, september months very low campaign and Most of the customer contact done by cellular mode. Most of the outcomes are unknown category and very few success.
*   Most of the customers not having personal loan. 55.6 % customers have the housing loan and 44.4 % customers not having housing loan. 98.2 % customers not having credit.
*   Most of the contacts were performed first and second time in the campaign. most of the customers not contacted before the campaign. 11.7 % clients only subscribed the term deposit remaining 88.3% not subcribed. Most of the outcomes are unknown category and very few success. Clients are interested in initial duration of calls 
*   Almost there are no correlation among the independent variables. It is identified that the balance and duration has negative correlation that indicates that the customers who are rich are spending less time on a call. Similarly campaign and duration has also negatively correlated.

**From the ML Model Implementation**

*   The Logistic Regression model performs better than other models such as Decision Tree, Naïve Bayes, K Nearest Neighbours. The Proposed Logistic Regression model have the Accuracy: 81.6 %, Precision :83.86 %, Recall: 78.26 %, F1 Score : 80.96 %, Cohens Kappa Score : 63.2 % and Area Under Curve : 89.98 %. Which are more compared to  aforementioned other models.

















