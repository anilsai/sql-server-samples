# Build a predictive model with Python using SQL Server 2017 Machine Learning Services

This sample shows how to create a predictive model in Python and operationalize it with SQL Server vNext.

### Contents

[About this sample](#about-this-sample)<br/>
[Before you begin](#before-you-begin)<br/>
[Sample details](#sample-details)<br/>
[Related links](#related-links)<br/>


<a name=about-this-sample></a>

## About this sample

Predictive modeling is a powerful way to add intelligence to your application. It enables applications to predict outcomes against new data.
The act of incorporating predictive analytics into your applications involves two major phases: 
model training and model operationalization.

In this sample, you will learn how to create a predictive model in python and operationalize it with SQL Server vNext.


<!-- Delete the ones that don't apply -->
- **Applies to:** SQL Server 2017 CTP2.0 or higher
- **Key features:**SQL Server Machine Learning Services 
- **Workload:** SQL Server Machine Learning Services
- **Programming Language:** T-SQL, Python
- **Authors:** Nellie Gustafsson
- **Update history:** Getting started tutorial for SQL Server ML Services - Python 

<a name=before-you-begin></a>

## Before you begin

To run this sample, you need the following prerequisites: </br>
Download a DB backup file and restore it using Setup.sql. [Download DB](https://deve2e.azureedge.net/sqlchoice/static/TutorialDB.bak)

**Software prerequisites:**

<!-- Examples -->
1. SQL Server 2017 CTP2.0 (or higher) with Machine Learning Services (Python) installed
2. SQL Server Management Studio
3. Python Tools for Visual Studio

## Run this sample
1. From SQL Server Management Studio or SQL Server Data Tools connect to your SQL Server vNext database and execute setup.sql to restore the sample DB you have downloaded </br>
2. From SQL Server Management Studio or SQL Server Data Tools, open the Predictive Model Python.sql script </br>
This script sets up: </br>
Necessary tables </br>
Creates stored procedure to train a model </br>
Creates a stored procedure to predict using that model </br>
Saves the predicted results to a DB table </br>
3. You can also try the python script on its own. Just remember to point the Python environment to the corresponding path "C:\Program Files\Microsoft SQL Server\MSSQL14.MSSQLSERVER\PYTHON_SERVICES" if you run in-db Python Server, or 
"C:\Program Files\Microsoft SQL Server\140\PYTHON_SERVER" if you have the standalone Machine Learning Server installed.

<a name=sample-details></a>

## Sample details

This sample shows how to create a predictive model with Python and generate predictions using the model and deploy that in SQL Server with SQL Server Machine Learning Services. 

### rental_prediction.py
The Python script that generates a predictive model and uses it to predict rental counts

###  rental_prediction.sql
Takes the Python code in Predictive Model.py and deploys it inside SQL Server. Creating stored procedures and tables for training, storing models and creating stored procedures for prediction.








