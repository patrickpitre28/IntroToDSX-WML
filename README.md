# DSX Cloud Introduction To DSX and WML

**Objective**

The objective of this lab is to introduce you to working with Jupyter Notebooks in DSX, to build a predictive model with Spark machine learning API (SparkML) to predict customer churn, and deploy it for scoring in Watson Machine Learning (WML).

**This repository contains the following assets**
1. ![Notebook](Notebooks)
2. ![Data](data)


**Demo setup**
1. Create a DSX project and name it "*DSX Lab - Telco Churn*"
2. Import ![Data](data) <br/>
Tip: First download the csv files before importing them into your project.  When downloading the csv files, make sure to click the **Raw** button to display the data in its raw format, right-click and select "Save Page As".
![Download CSV files](static/img/download_file.png?raw=true)

3. Import notebook <br/>
Within the "DSX Local Lab - Telco Churn" project, add a Notebook and choose to import it from this URL: https://github.com/SidneyPhoon/IntroToDSX-WML/blob/master/notebooks/PredictChurn-Build%20and%20Deploy%20to%20WML.ipynb

4. Follow instructions in the notebook and work through the "*PredictChurn-Build and Deploy to WML*" notebook

### Optional Lab Exercises

#### 1. Access data in flat files
- Download ![churn.csv](data/churn.csv?raw=true) and ![customer.csv](data/customer.csv?raw=true), and add them into the *DSX Lab - Telco Churn* project
- Create a duplicate of the "*PredictChurn-Build and Deploy to WML*" notebook

![Duplicate a notebook](static/img/duplicate_notebook.png?raw=true)

- Edit the "*PredictChurn-Build and Deploy to WML*" notebook to read the data from the flat files
- **Tip**: make sure *inferSchema* is set to 'true' when reading in the csv files, otherwise, all columns will be treated as String values.

![infer schema](images/infer_schema.png?raw=true)
