# Capstone_Project_AClinton

> Use predictive modeling techniques to determine the future of drug store sales after the COVID-19 pandemic. 

## Goals

- Set up a working Python environment
- Create a GitHub repo for the Capstone Project
- Research and discover useful data for the project goals
- Use machine learning, predictive modeling techniques to complete the project purpose. 

## Find Data

-Data found at https://www.census.gov/econ/currentdata/?programCode=MRTS&startYear=2018&endYear=2022&categories[]=4521E&dataType=SM&geoLevel=US&adjusted=1&notAdjusted=1&errorData=0

-Select the following to find the correct data: 
  1. Monthly Retail Trade and Food Service 
  2. Start: 2018  End: 2022
  3. 44611: Pharmacies and Drug Stores
  4. Sales: Monthly OR Sales: Monthly Percent Change
  5. U.S. Total

-Uncheck Seasonally Adjusted

-Click: Get Data

-Scroll to the bottom of the page where a table has appeared, providing requested data. 

-Download data as XLS-H (horizontal excel table): one table for monthly sales and one table for percent change

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

-Import data using pd.read_csv *Ensure you are loading a csv file, not an xls file.

-Create the dataframe using pd.DataFrame. Load data, and identify columns. 

-Complete a basic view/analysis of the loaded dataframe. *This should include using df.head, df.describe, and any relevant updates/initial graphs. For this project, total sales revenue for each year was calculated using the .sum() function. Matplotlib was imported and used to create scatter plots for total sales data and total percent change data as well as a plot for comparison of each year's sales data by month. 

### Prepare data for predictive analysis

