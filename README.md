# HR-Dataset
This project aims to analyze and visualize Performance of Employees data in the Company for the years 2012-2022. The data is sourced from the HR_dataset and has been processed using Power BI for easy management and analysis.This project showcases our skills in Power BI as I go through data cleaning, analysing and visualizing the layoffs dataset.
## Table of Contents

- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Data Analysis](#data-analysis)
- [Visualizations](#visualizations)
- [Limitations/Assumptions](#limitationsassumptions)
  
## Data Sources
The layoffs dataset was sourced from Google Drive . You can find the raw file at https://drive.google.com/drive/folders/1F6OBnq8BEPWrkvGa9n0ZKLM7CIemSnVw

## Tools
- Power  Query( ETL, Conditional Columns, Custom Columns using M Language)
- Power Pivot (DAX)
- Data Modeling

## Data Cleaning
Here's the updated README file with the additional details on renaming unclear titles, capitalizing each word in columns, and merging first and last names:

markdown
# HR Analytics Power BI Project

## Overview
This Power BI project focuses on analyzing HR data to gain insights into employee demographics, performance, and training opportunities. The project uses several tools and techniques within Power BI to achieve this.

## Tools and Techniques Used

### 1. Data Cleaning
- **Setting the First Row as Header**:
  - Navigate to the 'Transform Data' tab.
  - Select the option to use the first row as headers (Home > Use First Row as Headers).
  
- **Removing Null Values**:
  - In the 'Transform Data' tab, select the columns where you want to remove nulls.
  - Use the 'Remove Rows' drop-down menu (Home > Remove Rows > Remove Rows with Errors).
  
- **Removing Empty Columns**:
  - In the 'Transform Data' tab, select the columns you want to remove.
  - Use the 'Remove Columns' option (Home > Remove Columns > Remove Empty Columns).

- **Renaming Unclear Titles**:
  - Navigate to the 'Transform Data' tab.
  - Double-click on the column headers you want to rename and provide clear and descriptive titles.

- **Capitalizing Each Word in Columns**:
  - Navigate to the 'Transform Data' tab.
  - Select the column you want to capitalize.
  - Use the 'Format' option (Transform > Format > Capitalize Each Word).

- **Merging First and Last Name Columns into Full Name**:
  - Navigate to the 'Transform Data' tab.
  - Select the first and last name columns.
  - Use the 'Merge Columns' option (Transform > Merge Columns) and choose a separator (e.g., space) to create a full name column.

### 2. Conditional Columns
- **Age Categories**: We created a conditional column to classify employees into different age categories based on their ages.
  - **Categories**: 
    - Young Adult (18-29)
    - Middle Adult (30-39)
    - Older Adult (40-51)
  - **Steps**:
    - Navigate to the 'Transform Data' tab.
    - Select 'Add Column' > 'Conditional Column'.
    - Define the conditions and corresponding outputs for different age groups.

- **Distance Categories**: We created a conditional column to group employees based on their distance from the office.
  - **Categories**: 
    - Nearby (1-15)
    - Far (16-30)
    - Very Far (31-45)
  - **Steps**:
    - Navigate to the 'Transform Data' tab.
    - Select 'Add Column' > 'Conditional Column'.
    - Define the conditions and corresponding outputs for different distance ranges.

### 3. Custom Columns using M Language
- **Percentage of Training Opportunities Taken**: We used M Language to create a custom column that calculates the percentage of training opportunities taken by each employee.
  - **Steps**:
    - Navigate to the 'Transform Data' tab.
    - Select 'Add Column' > 'Custom Column'.
    - Enter the M Language formula to calculate the percentage. An example formula might look like:
      m
      if [Total Training Opportunities] = 0 then 0 else [Training Taken] / [Total Training Opportunities] * 100
      

## Conclusion
This README provides an overview of the key tools and techniques used in our HR analytics Power BI project. By utilizing data cleaning, conditional columns, and custom columns with M Language, we were able to categorize and analyze employee data effectively.


Feel free to edit and expand on this draft to best suit your project details. Let me know if there's anything else you need!






