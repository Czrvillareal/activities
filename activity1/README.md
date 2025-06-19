# COSC 110 ACTIVITY NO. 1
This project provides an exploratory data analysis of the Titanic dataset, focusing on initial data inspection, handling missing values, and analyzing survival patterns using computational thinking principles.

## Project Goal
 The primary objective was to apply computational thinking (Decomposition, Pattern Recognition, Abstraction, Algorithm Design) to a real-world dataset. This involved:
 - Loading and inspecting the dataset structure.
 - Identifying and strategizing on handling missing data.
 - Analyzing passenger survival rates based on key features like Sex, Pclass, and Age.

## Dataset
The analysis uses the classic Titanic dataset, sourced from: [Kaggle's Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)

## Analysis Highlights & Computational Thinking
The complete code and detailed steps can be found in the associated Jupyter Notebook. Below is a summary of the questions and actions done:

### Question 1: What are the underlying tasks needed for loading and handling the data?
 - Dataset Preparation: Identifying titanic.csv.
 - Library Import: Importing pandas and matplotlib.pyplot.
 - Data Access: Loading the CSV from the specified URL.
 - Initial Inspection: Using df.head(), df.shape (891 rows, 12 columns), and df.info() for a preliminary overview.

### Question 2: Which columns contain missing values? Should we remove or fill them?
 - Columns with Missing Values: Age (177 missing), Cabin (687 missing), Embarked (2 missing).
 - Strategy (Algorithm Logic):
   - Cabin: High number of missing values and non-numeric; consider removal or an indicator feature.
   - Age: Significant for analysis; imputation (filling) is preferred to avoid bias.
   - Embarked: Small number; can be filled (e.g., mode) or removed.
     
### Question 3: What is the survival rate of all passengers in the dataset? What can you deduce?
 - Overall Survival Rate: 38.38% (less than half survived).
 - Deductions:
   - By Sex: Females (74.20%) had a significantly higher survival rate than males (18.89%).
   - By Passenger Class (Pclass): Survival rates correlated directly with class: First (62.96%), Second (47.28%), Third (24.24%).
   - Overall Deduction: Gender and socio-economic status (represented by Pclass) were strong factors in survival.

### Question 4: What is the average age of the survivors and non-survivors in the dataset?
 - Average Age of Survivors: 28.34 years
 - Average Age of Non-Survivors: 30.63 years
 - Methodology: Data was segmented by Survived status, average age calculated for each group, and age distributions visualized using histograms for general trends.

> Assisted by Gemini.
