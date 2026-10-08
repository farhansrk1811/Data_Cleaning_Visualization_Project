# Data Cleaning & Visualization Project

## Project Overview

This project focuses on cleaning, analyzing, and visualizing an employee dataset using Python.

The dataset contains employee information such as name, age, salary, joining date, and department.

## Objectives

- Inspect the raw dataset
- Identify missing values and duplicate records
- Handle missing data
- Detect and handle salary outliers
- Convert date fields into the correct format
- Create useful derived columns
- Perform exploratory data analysis
- Create meaningful visualizations

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code

## Dataset

The original dataset contains 43 records and 5 columns.

After data cleaning, the dataset contains 42 records and 7 columns.

### Original Columns

- Name
- Age
- Salary
- Join_Date
- Department

### Additional Columns Created

- Join_Year
- Age_Group

## Data Cleaning Performed

The following cleaning activities were performed:

1. Checked the structure and data types of the dataset.
2. Identified missing values.
3. Removed one genuine duplicate record.
4. Filled missing Age values using the median Age.
5. Filled missing Salary values using the median Salary.
6. Detected salary outliers using the IQR method.
7. Capped salary outliers at the calculated upper IQR limit.
8. Converted Join_Date into datetime format.
9. Created Join_Year from Join_Date.
10. Created Age_Group based on employee age.

## Visualizations

The project includes the following visualizations:

1. Employee Count by Department
2. Salary Distribution
3. Average Salary by Department
4. Age Distribution
5. Salary by Department
6. Age vs Salary
7. Employees by Joining Year
8. Correlation Heatmap

## Project Structure

```text
Data_Cleaning_Visualization_Project
│
├── Dataset
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── Visualizations
│   ├── department_distribution.png
│   ├── salary_distribution.png
│   ├── average_salary_department.png
│   ├── age_distribution.png
│   ├── salary_by_department.png
│   ├── age_salary_scatter.png
│   ├── employees_joining_year.png
│   └── correlation_heatmap.png
│
├── data_cleaning_visualization.ipynb
└── README.md