## Comparative Drug Performance on Treating Tumors in Mice
Analyzes Pharmaceutical Data Using Pandas and MatPlotLib

## Objectives:
In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens. This project generates all of the tables and figures needed for the technical report of the clinical study.

### Step 1 - Prepare the Data
- Merge the mouse_metadata and study_results DataFrames into a single DataFrame

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/3771057e-bd39-423f-a991-fba48c9f9474)

- Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points
- Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed
- Display the updated number of unique mice IDs

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/da7db058-1261-485e-ad60-94da937c0997)

### Step 2 - Generate Summary Statistics
- Create a DataFrame of summary statistics including a row for each drug regimen and a column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/a034c8e3-b86d-46e7-91bf-bce5857c527a)

### Step 3 - Create Bar Charts and Pie Charts
- Generate two bar charts that show the total number of time points for all mice tested for each drug regimen throughout the study
  - Create the first bar chart with the Pandas DataFrame.plot() method.

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/d022759f-2d14-4bd8-a56d-450c460cd93e)

* Create the second bar chart with Matplotlib's pyplot methods.    
![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/42628c62-7c23-456a-a5c8-85c3331d4628)

- Generate two pie charts that show the distribution of female versus male mice in the study.
  - Create the first pie chart with the Pandas DataFrame.plot() method.

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/a0c8e6a8-92d5-4a19-aeee-a5076dac571c)

* Create the second pie chart with Matplotlib's pyplot methods.    

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/3a580c47-dbc8-44ff-bdc8-4f699973fcee)

### Step 4 - Calculate Quartiles, Find Outliers, and Create a Box Plot
- Create a grouped DataFrame that shows the last (greatest) time point for each mouse
  - Merge this grouped DataFrame with the original cleaned DataFrame
- Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data
- Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment
- Append the resulting final tumor volumes for each drug to the empty list
- Determine outliers by using the upper and lower bounds Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group
  - Highlight any potential outliers in the plot by changing their color and style

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/db95df3a-00e2-4809-8ade-e1c223c93b4c)

### Step 5 - Create a Line Plot and a Scatter Plot
- Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse
![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/88939999-9925-421d-9674-2d03314ea187)

- Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen
![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/60d2004f-b95a-4199-923d-dc305cb482b8)

### Step 6 - Calculate Correlation and Regression
- Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment
- Plot the linear regression model on top of the previous scatter plot

![image](https://github.com/antara2022/Comparative-Drug-Performance-on-Treating-Tumors-in-Mice/assets/112270155/82118dda-3927-4001-b1b4-6ae227851e12)

Contact: antara.choudhury3000@gmail.com
