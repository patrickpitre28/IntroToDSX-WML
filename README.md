# DSX Cloud Introduction To DSX and WML

**Objective**

The objective of this lab is to introduce working with Jupyter Notebooks in DSX to build a predictive model with Spark machine learning API (SparkML) to predict customer churn, and deploy it for scoring in Watson Machine Learning (WML).

**This repository contains the following assets**
1. ![Notebook](Notebooks)
2. ![Data](data)


**Demo setup**
1. Create a DSX project and name it "*DSX Lab - Telco Churn*"
2. Import ![Data](data) <br/>
Tip: First download the csv files before importing them into your project.  When downloading the csv files, make sure to click the **Raw** button to display the data in its raw format, right-click and select "Save Page As".
![Download CSV files](static/img/download_csv.png?raw=true)

3. Import notebook <br/>
Within the "DSX Local Lab - Telco Churn" project, add a Notebook and choose to import it from this URL: https://github.com/elenalowery/DSX-Local-Telco-Churn/blob/master/Notebooks/Telco%20Churn%20ML_Local.ipynb

4. Follow instructions in the notebook to add project token, and work through the notebook
5. Optional: deploy Telco Churn UI application: instructions in the ![WebApp](WebApp) folder. Or you can use this deployed UI: https://predictcustomerchurnel.mybluemix.net/
6. If you would like to show Model Management - create several deployments from this or different notebooks
7. Optionally, watch a [video](https://ibm.box.com/s/9u40d8ug8paajh35ars0vtvhj48964wb) of the presentation and demo

**Demo**
1. Follow the agenda in the presentation 
2. During the demo show capabilities of DSX in the context of Telco Churn use case
   * Start with the overview of the use case and optionally the Telco Churn UI
   * Log in to DSX Local and create a new project
   * Show collaboration features for the project
   * Load data and explain what type of data sources are supported
   * Create a notebook from File
   * Walk through the notebook
   * Explain the deployment process - via UI and API
   * Test the model via UI or API and explian how the demo UI makes the same call
3. Wrap up with architecture discussion 
 
