# Capstone_Project_AClinton

> Use predictive modeling techniques to determine the future of drug store sales after the COVID-19 pandemic. 

## Goals

- Set up a working Python environment
- Create a GitHub repo for the Capstone Project
- Research and discover useful data for the project goals
- Use machine learning, predictive modeling techniques to complete the project purpose. 

## Find Data

*Data found at https://www.census.gov/econ/currentdata/?programCode=MRTS&startYear=2018&endYear=2022&categories[]=4521E&dataType=SM&geoLevel=US&adjusted=1&notAdjusted=1&errorData=0

Select the following to find the correct data: 

  1. Monthly Retail Trade and Food Service 
  2. Start: 2018  End: 2022
  3. 44611: Pharmacies and Drug Stores
  4. Sales: Monthly OR Sales: Monthly Percent Change
  5. U.S. Total
  
Uncheck Seasonally Adjusted

Click: Get Data

Scroll to the bottom of the page where a table has appeared, providing requested data. 

Download data as XLS-H (horizontal excel table): one table for monthly sales and one table for percent change

## Prepare Data

Merge both xls files into one and clean data as needed. For this project, an additional row was added to represent annual percent change and annual sales revenue. 

-Once merged, remove duplicated title rows 

-Add annual percent change row

-Add annual sales row 

-Convert xls file to csv format

-Upload data to repo

## Jupyter Notebook and Analysis of Data

Open a new command prompt and move to relevant folder on local computer(this should be a folder in which all relavent documents, images, and project information is stored). Once in the correct folder location, connect to Jupyter Lab. Upon launch of Jupyter Lab, open a new notebook and rename to reflect the project. 
In the new notebook:

-Import pandas as pd

-Import data using pd.read_csv _Ensure you are loading a csv file, not an xls file._

-Create the dataframe using pd.DataFrame. Load data, and identify columns. 

-Complete a basic view/analysis of the loaded dataframe. _This should include use of df.head, df.describe, and any relevant updates/initial graphs. For this project, total sales revenue for each year was calculated using the .sum() function. Matplotlib was imported and used to create scatter plots for total sales data and total percent change data as well as a plot for comparison of each year's sales data by month. _

### Prepare data for predictive analysis

Import the following modules:

  -Pandas as pd(imported above)

  -Matplotlib.pyplot as plt(imported above)

  -Numpy as np

  -Import seaborn as sn
 
  -From sklearn.model_selection
    
    train_test_split
    
  -From sklearn.linear_model
    
    LinearRegression
    
    ElasticNet

  -From sklearn.preprocessing
  
    PolynomialFeatures

  -From sklearn.metrics
  
    mean_squared_error
  
    mean_absolute_error
  
    r2_score

Split data into a train and test model using the train_test_split module. Print train set and test set. Create useable train and test sets by using 're-index' to list data in order by month and convert month from string to numerical data using .replace(). Begin analysis using linear regression for each of the five years, multiple regression, polynomial regression at powers of one, two, and three, and elastic net models at powers of there and eight. 

Transfer results of each model to an excel file. Using excel visualizations, create graphs to present and compare each model and related data. Using predicted y-values, graph each predicted value in comparison to actual values. Analyze and compare all models and data to determine which test provides best fit for project goals. 

For this project, multiple regression model, polynomial regression model with a power of two, and polynomial regression model with a power of three represent the data and project goals best. 

Link to Overleaf Project: https://www.overleaf.com/read/mjpkmjcbdkmx
