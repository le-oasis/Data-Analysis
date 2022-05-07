# Data-Analysis

## Project:0 - IMDB Movie Dataset Exercise Solutions | Pandas Project | Kaggle Dataset

Dataset Link:https://www.kaggle.com/datasets/PromptCloudHQ/imdb-data

Questions: 
1. Display Top 10 Rows of The Dataset
2. Check Last 10 Rows of The Dataset
3. Find Shape of Our Dataset (Number of Rows And Number of Columns)
4. Getting Information About Our Dataset Like Total Number Rows, Total Number of Columns, Datatypes of Each Column And Memory Requirement
5. Check Missing Values In The Dataset
6. Drop All The  Missing Values
7. Check For Duplicate Data
8. Get Overall Statistics About The DataFrame
9. Display Title of The Movie Having Runtime Greater Than or equal to 180 Minutes
10. In Which Year There Was The Highest Average Voting?
11. In Which Year There Was The Highest Average Revenue?
12. Find The Average Rating For Each Director
13. Display Top 10 Lengthy Movies Title and Runtime
14. Display Number of Movies Per Year
15. Find Most Popular Movie Title (Highest Revenue)
16. Display Top 10 Highest Rated Movie Titles And its Directors

17. Display Top 10 Highest Revenue Movie Titles
18.  Find Average Rating of Movies Year Wise
19. Does Rating Affect The Revenue?
20. Classify Movies Based on Ratings [Excellent, Good, and Average]
21. Count Number of Action Movies
22. Find Unique Values From Genre 
23. How Many Films of Each Genre Were Made?


## Project:1 -  Supermarket Sales Data 

Dataset Link: https://github.com/le-oasis/Data-Analysis/blob/main/sales_data.csv

Problem Statment:
In the year 2013, a supermarket decided to draw insight from their data in order to make data driven decisions. As a Data Analyst,you are presented with their 2013 daily sales records (sales_data.csv) and tasked to help them find answers to the questions below by analysing the data.

i. What is the average sales and profit per market?

ii.Plot a stacked bar chart showing the sales and profit per market.

iii.Which market brings more sales on the average?

i. What are the best 10 performing products with regards to sales in 2013?

ii.What are the least 10 performing products with regards to sales 2013?

i. Extract the days and months from the Order Date and add them to the data frame with the name "Days" and "Months" respectively?

ii.Show the trend of profit from January to December with a line plot.

iii. Which month does the company make more profit and what 5 products are sold most in that month? iv. which day does the company make high sales on the average?

i. By analyzing the data, what is the correlation between sales and discount?

ii. Use a scatter plot to show the relationship between sales and profit.

i. Plot a grouped bar chart showing the total profit for the different product category for each market. ii. From your graph, which product category performs well in each market?

i. Which customer spent the most in the whole year? ii. What product does the customer in (i) buy the most? iii. Which month did the customer spent the most? iv. How much did this customer spend in the whole year?

Can you do any other analysis to draw more insight? Feel free to do it.


## Project:2 - Telecommunications Dataset Exercise Solutions | Pandas Project


You are given three data sets which contain different information about customers in a telecommunications company.
In all datasets, each row represents a customer and the columns contains that customer's individual attributes. 
Your task is to perform explanatory analysis and data manipulation.


In order to complete the task you must write a function named explanatory_analysis() that takes three arguments, charges_data_path, personal_data_dath, and plan_data_path, which are the paths to the respective datasets.

The function should perform the following steps:

Read all three datasets.
charges_data has some missing values in the monthlyCharges and totalCharges columns.
Fill in the missing values in the monthlyCharges column with the trimmed average of non-empty observations from this column. To calculate a trimmed average, reject 10% of the biggest and 10% of the smallest values from calculations. Round the final value to the nearest integer.
Then fill in the missing values in the totalCharges column with the monthlyCharges value multiplied by the tenure value.
Create a new column, tenureBinned, by discretizing the original tenure column. The tenureBinned column should take the values group1, group2, group3 and group4 when the values of tenure are within the respective ranges (0, 24], (24, 48], (48, 60] and (60, Inf).
Calculate the churn rate, that is the percentage of churned customers, and round the result to the nearest integer e.g. If the fraction of such people in the dataset is 0.1234, then the desired value should be equal to 12.
Join the updated charges_data with personal_data by the customerID column so that the resulting dataset has only rows with common customer IDs. Then, join the resulting dataset with plan_data by customerID, this time leaving all rows from the first dataset (joined charges_data and personal_data).
Using the merged data, calculate the percentage of customers who are more than 60 years old and round the result to the nearest integer; e.g. if the fraction of such people in the dataset is 0.6789, then the desired value should be equal to 68.
Using the merged data , create a dictionary containing counts of unique values in the internetService column, where keys are the unique values of items and their counts.
The function exploratory_analysis() returns a dictionary with the following values:

monthly_charges_mean - an integer with a calculated trimmed average from monthlyCharges values (calculated before filling in missing values and including three missing values);
charges_data_updated - a dataframe with updated charges_data, that is with filled values in the columns monthlyCharges and totalCharges and an added tenureBinned column;
churn_pet - an integer with the churn rate (as a percentage);
data_merged - a data frame with three joined datasets;
pct_age_above_60 - an integer giving the percentage of customers older than 60;
internet_service_counts - a dictionary with InternetService value counts.
Package versions
Additionally to the Python 3.8 Standard Library, you may use the following packages:

Pandas
Numpy
Scipy
