# Itroduction To DSX Cloud and WML

**Objective**

The objective of this lab is to introduce you to working with Jupyter Notebooks in DSX, to build a predictive model with Spark machine learning API (SparkML) to predict customer churn, and deploy it for scoring in Watson Machine Learning (WML).  You will also build and deploy the same Spark ML model with the visual ML Model Builder interface, so that you can compare the programmatic approach to the visual model builder.

**This repository contains the following assets**
1. ![Notebooks](notebooks)
2. ![Data](data)

## Lab 1: Build and Deploy predictive model programmatically with Jupyter Notebook
**Lab setup**
1. Create a DSX project and name it "*DSX Lab - Telco Churn*"
2. Import ![Data](data) <br/>
**Tip**: First download the csv files before importing them into your project.  When downloading the csv files, make sure to click the **Raw** button to display the data in its raw format, right-click and select "Save Page As".
![Download CSV files](static/img/download_file.png?raw=true)

3. Import notebook <br/>
Within the "DSX Lab - Telco Churn" project, add a Notebook and choose to import it from this URL: https://github.com/SidneyPhoon/IntroToDSX-WML/blob/master/notebooks/PredictChurn-Build%20and%20Deploy%20to%20WML.ipynb

4. Follow instructions in the notebook and work through the "*PredictChurn-Build and Deploy to WML*" notebook

5. This is an example of a web application that makes REST API calls to a deployed model to predict customer churn in real-time, https://predictcustomerchurn.mybluemix.net/

<br/>

## Lab 2: Build and Deploy predictive model with the IBM ML visual interface
- In the *DSX Lab - Telco Churn* project, click **Settings**
- Scroll-down to **Associated Services**, select an instance of Machine Learning.  Associating an instance of ML service with the project allows you to deploy models built with visual tools, such as the ML Model Builder or Flows
- Go to **Analytics Assets** in the project
- In the **Models** section click *Add Model*
- Follow the visual guide to build a Spark ML model to preduct churn.  The input file is **customer_churn.csv** file.  This file contains the merged data from the customer.csv and churn.csv.  Choose *Automatic* if you want ML to build and pick the best performing model for you, choose *Manual* if you want to choose the your own models
- When the model is built, click *Save* to save the model into the WML repository
![infer schema](static/img/model_builder_save_model.png?raw=true)
- Click **Add Deployment** to create and Online deployment
- Click the **Predictions** tab to the the visual interface for testing your deployed model
-  The values for testing are,<br/> ID=999, Gender=F, Status=M, Children=2, EstIncome=80000, CarOwner=Y, Age=33, LongDistance=40, International=0, Local=50, Dropped=1, Paymethod=CC, LocalBilltype=Budget, LongDistanceBilltype=Standard, Usage=65, RatePlan=2


### Optional Lab Exercises

#### 1. Access data in flat files
- Download ![churn.csv](data/churn.csv?raw=true) and ![customer.csv](data/customer.csv?raw=true), and add them into the *DSX Lab - Telco Churn* project
- Create a duplicate of the "*PredictChurn-Build and Deploy to WML*" notebook

![Duplicate a notebook](static/img/duplicate_notebook.png?raw=true)

- Edit the "*PredictChurn-Build and Deploy to WML*" notebook to read the data from the flat files
- **Tip**: make sure *inferSchema* is set to 'true' when reading in the csv files, otherwise, all columns will be treated as String values.

![infer schema](static/img/infer_schema.png?raw=true)
<br/>




