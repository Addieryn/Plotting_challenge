# Plotting_challenge
What good is data without a good plot to tell the story? <br>
In this assignment, you’ll apply what you've learned about Matplotlib to a real-world situation and dataset. 
## Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anticancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer. <br>
As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens. <br>
The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results. 
## Files
Download the following files to help you get started: <br>
Module 5 Challenge files Links to an external site. 
## Instructions
This assignment is broken down into the following tasks: <br>
Prepare the data. <br>
Generate summary statistics. <br>
Create bar charts and pie charts. <br>
Calculate quartiles, find outliers, and create a box plot. <br>
Create a line plot and a scatter plot. <br>
Calculate correlation and regression. Submit your final analysis. 
## Prepare the Data
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame. <br>
Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new <br>
DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps. <br>
Display the updated number of unique mice IDs. 
## Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result. <br>
Your summary statistics should include: <br>
A row for each drug regimen. These regimen names should be contained in the index column. A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume. 
## Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study. <br>
Create the first bar chart with the Pandas DataFrame.plot() method. <br>
Create the second bar chart with Matplotlib's pyplot methods. <br>
Generate two pie charts. Both charts should be identical and show the distribution of unique female versus male mice in the study. <br>
Create the first pie chart with the Pandas DataFrame.plot() method. <br>
Create the second pie chart with Matplotlib's pyplot methods. 
## Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps: <br>
Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame. <br>
Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data. <br>
Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list. <br>
Determine outliers by using the upper and lower bounds, and then print the results.<br> 
Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style. <br>
hint: All four box plots should be within the same figure. Use this [Matplotlib documentation page](https://matplotlib.org/stable/gallery/statistics/boxplot_demo.html) for help with changing the style of the outliers. 
## Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse. <br>
Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen. 
## Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen. Plot the linear regression model on top of the previous scatter plot. 
## Requirements
#### Prepare the Data (20 points) 
The datasets are merged into a single DataFrame. (6 points) <br>
The number of mice are shown from the merged DataFrame. (2 points) <br>
Each duplicate mice is found based on the Mouse ID and Timepoint. (6 points) <br>
A clean DataFrame is created with the dropped duplicate mice. (4 points) <br>
The number of mice are shown from the clean DataFrame. (2 points) 
#### Generate Summary Statistics (15 points) 
The mean of the tumor volume for each regimen is calculated using groupby. (2 points) <br>
The media of the tumor volume for each regimen is calculated using groupby. (2 points) <br>
The variance of the tumor volume for each regimen is calculated using groupby. (2 points) The standard deviation of the tumor volume for each regimen is calculated using groupby. (2 points) <br>
The SEM of the tumor volume for each regimen is calculated using groupby. (2 points)<br> 
A new DataFrame is created with using the summary statistics. (5 points) 
#### Create Bar Charts and Pie Charts (15 points) 
A bar plot showing the total number of timepoints for all mice tested for each drug regimen using Pandas is generated. (4.5 points) <br>
A bar plot showing the total number of timepoints for all mice tested for each drug regimen using pyplot is generated. (4.5 points) <br>
A pie chart showing the distribution of unique female versus male mice using Pandas is generated. (3 points) <br>
A pie chart showing the distribution of unique female versus male mice using pyplot is generated. (3 points) 
#### Calculate Quartiles, Find Outliers, and Create a Box Plot (30 points) 
A DatFrame that has the last timepoint for each mouse ID is created using groupby. (5 points) <br>
The index of the DataFrame is reset. (2 points) <br>
Retrieve the maximum timepoint for each mouse. (2 points) <br>
The four treatment groups, Capomulin, Ramicane, Infubinol, and Ceftamin, are put in a list. (3 points) <br>
An empty list is created to fill with tumor volume data. (3 points) <br>
A for loop is used to display the interquartile range (IQR) and the outliers for each treatment group (10 points) <br>
A box plot is generated that shows the distribution of the final tumor volume for all the mice in each treatment group. (5 points) 
#### Create a Line Plot and a Scatter Plot (10 points) 
A line plot is generated that shows the tumor volume vs. time point for one mouse treated with Capomulin. (5 points) <br>
A scatter plot is generated that shows average tumor volume vs. mouse weight for the 
Capomulin regimen. (5 points) <br>
#### Calculate Correlation and Regression (10 points) 
The correlation coefficient and linear regression model are calculated for mouse weight and average tumor volume for the Capomulin regimen. (10 points) 
