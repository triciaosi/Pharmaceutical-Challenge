# Pharmaceutical-Challenge
# Background

I just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, I've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

# Steps I took to analyze my data:

* Prepare the data.

* Generate summary statistics.

* Create bar charts and pie charts.

* Calculate quartiles, find outliers, and create a box plot.

* Create a line plot and a scatter plot.

* Calculate correlation and regression.

## Prepare the Data
1. I ran the provided package dependency and data imports, and then merged the mouse_metadata and study_results DataFrames into a single DataFrame.
2. I displayed the number of unique mice IDs in the data, and then checked for any mouse ID with duplicate time points. 
3. Next I Displayed the data associated with that mouse ID, and then created a new DataFrame where this data is removed. 
4. I then this cleaned DataFrame for the remaining steps.
5. Lastly, I displayed the updated number of unique mice IDs.

## Generate Summary Statistics
* I created a DataFrame of summary statistics. 

* My summary statistics includes: 
  * A row for each drug regimen. These regimen names should be contained in the index column.
  * A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

## Create Bar Charts and Pie Charts
* I generated two bar charts: 
  * The first bar chart was created with the Pandas DataFrame.plot() method.
  * The second bar chart was created using Matplotlib's pyplot method.

* I generate two pie charts, that each show the distribution of female versus male mice in the study.
  * The first pie chart was created with the Pandas DataFrame.plot() method.
  * The second pie chart was created using Matplotlib's pyplot methods.

# Calculate Quartiles, Find Outliers, and Create a Box Plot
* I calculated the final tumor volume of each mouse across four of the most promising treatment regimens: 
  * Capomulin, Ramicane, Infubinol, and Ceftamin.
* Then, I calculated the quartiles and IQR, and determined if there were any potential outliers across all four treatment regimens. 


# Create a Line Plot and a Scatter Plot
* I selected a mouse that was treated with Capomulin, and generated a line plot of tumor volume versus time point for that mouse.
* Next, I generated a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

# Calculate Correlation and Regression

* I calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.
* Lastly, I plotted the linear regression model on top of the previous scatter plot.

