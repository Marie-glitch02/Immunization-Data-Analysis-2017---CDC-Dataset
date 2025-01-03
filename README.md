# Immunization Data Analysis (2017) - CDC Dataset

## Overview

This project explores the 2017 immunization data from the Centers for Disease Control and Prevention (CDC) to analyze various aspects of children's immunization status. The analysis examines relationships between vaccination rates, demographic factors like mother’s education level, breastfeeding, and disease occurrences like chickenpox.

The dataset used in this project is contained in the file `NISPUF17.csv`
## Tasks

This repository focuses on solving several tasks based on the dataset:

### 1. Proportion of Education Levels
Write a function called `proportion_of_education` that calculates the proportion of children based on the education level of their mothers. The function categorizes mothers into:
- **Less than high school**: `< 12 years`
- **High school**: `12 years`
- **More than high school but not college**: `> 12 years but < 16 years`
- **College**: `>= 16 years`

The function returns a dictionary with the proportions for each category.
<p align=center><img width="602" alt="mother-education-level" src="https://github.com/user-attachments/assets/54665552-59c3-408d-b90d-5a56b5518033" /> </p>

### 2. Breastmilk and Influenza Vaccination
Write a function to calculate the average number of seasonal influenza vaccinations received by children who were fed breastmilk versus those who were not fed breastmilk.
<p align=center><img width="415" alt="influenza-vaccines" src="https://github.com/user-attachments/assets/ab0f0d5a-f741-4bce-b1b7-9ba5c1ad2a99" /></p>

### 3. Vaccine Effectiveness and Gender
Write a function to analyze the relationship between vaccine effectiveness (based on varicella doses) and the sex of the child. The function calculates the ratio of children who contracted chickenpox but were vaccinated against it, comparing this ratio by sex.

### 4. Correlation Between Chickenpox and Vaccine Doses
Calculate the correlation between having had chickenpox and the number of varicella vaccine doses given. The function also calculates the p-value to assess the statistical significance of the correlation.
### 5. Visualization: 
To visualize the number of doses for different vaccines in the dataset, creating a bar plot to compare the total number of doses for each vaccine
<p align=center><img width="524" alt="total-number-of-vaccines" src="https://github.com/user-attachments/assets/e7701b17-e86e-4510-9eb7-30501a059e87" /></p>

## Dataset Access

- **CSV File**: `assets/NISPUF17.csv`

## Requirements

- **Python** 3.x
- **Pandas**: For data manipulation and analysis
- **NumPy**: For numerical calculations
- **SciPy**: For statistical analysis (correlation and p-value)

## Functions

### 1. `proportion_of_education(df)`
This function calculates the proportion of children based on the education level of their mothers. It returns a dictionary with the following keys:
- `"less than high school"`
- `"high school"`
- `"more than high school but not college"`
- `"college"`

### 2. `average_influenza_vaccine_by_breastmilk(df)`
This function calculates the average number of seasonal influenza vaccines received by children who were breastfed versus those who were not.

### 3. `vaccine_effectiveness_by_sex(df)`
This function calculates the ratio of children who contracted chickenpox but were vaccinated against it (at least one varicella dose) versus those who did not contract chickenpox, breaking it down by sex.

### 4. `correlation_chickenpox_and_vaccine_doses(df)`
This function calculates the correlation between having had chickenpox and the number of varicella vaccine doses given, along with the p-value to assess the statistical significance.


