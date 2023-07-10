# final_project
DA2 Southern Indiana capstone project
# Capstone 2 - Examination of LFD Fire Incident Damage Reporting

### The goal of this project is to combine Fire incident reporting with property damage data, therefore creating a comparative ratio of property saved vs damaged during fire incidents LFD responded to in the year 2017. Ideally a broad view visual will be provided with the option for a user input for specific station detailed visual.

### requirements pandas, matplotlib, python 3.10.10

### 1. Read data in. 
    Read in data from a local csv, excel file, json, or any other file type.
    
    Two csv files read in with pandas.

### 2. Manipulate and clean your data.
    Use custom functions or lambdas to perform specific operations to clean or manipulate your data, return those values, 
    then use them in other parts of your project.
    
    Inner Join completed with a merge function on specific columns needed for calculations and de-duped. Noted inconsistent reporting in Saved column with negative values that were stored as varchar. Changed dtype to str in order to replace all negative values to zero and then changed dtype back to numeric for aggregation.

### 3. Analyze your data!
    Write custom functions to operate on your data.
    
    Created input function to allow user to select a station by number only and recieve a visualize comparison of loss vs saved property based on sum of values of each stations reportings. 
    Visualized average value of properties responded to based on Stations that serviced the incident.
    
### 4. Visualize your data.
    Make 2 basic plots with matplotlib, seaborn, etc.
   
    Utilized pandas and matplotlib to generate pie charts from user input selection, and a bar chart overview of all reported stations damage/save ratio, Bar chart comparison of average property values.
    
### 5. Interpret your data and graphical output. If your project is in a Jupyter Notebook, this should be between the important cells.
    Write markdown cells in Jupyter explaining your thought process and code. If you make a few plots with matplotlib, 
    explain what the reader is seeing and why you chose to plot things that way.
