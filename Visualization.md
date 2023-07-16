# Titanic Dataset Preprocessing and Visualization

This file contains code for preprocessing and visualizing the Titanic dataset. The goal is to prepare the data for machine learning and analyze some visual insights.

## Data Preprocessing

1. Load Data: The dataset is loaded into a Pandas DataFrame named 'titanic' from a CSV file named 'titanic.csv'.

2. Drop Columns: The 'Name' column is removed from the DataFrame since it is not directly relevant for survival prediction. The 'Fare' and 'Cabin' columns are also dropped as they do not contribute to predicting survival.

3. Gender Encoding: The 'Sex' column, which contains categorical values ('male' and 'female'), is converted to numeric values using two methods:
   - Using a custom function 'getNumber': 'male' is encoded as 1 and 'female' as 0.
   - Using Scikit-learn's 'LabelEncoder': The 'Sex' column is converted to binary values (1 for male, 0 for female).

4. Handling Missing Values: The missing values in the 'Age' column are filled with the mean age of passengers who survived and passengers who didn't survive. Afterward, any remaining rows with missing values are dropped from the DataFrame.

5. Embarked Encoding: The 'Embarked' column, which contains categorical values ('Q', 'S', 'C'), is converted to numeric values using Scikit-learn's 'LabelEncoder'.

## Data Visualization

1. Pie Chart for Gender: A pie chart is created to show the proportion of males and females in the dataset.

2. Pie Chart for Survival by Gender: A pie chart is created to display the percentage of males and females who survived and those who did not survive.

3. Bar Plot for SibSp vs. Survival: A bar plot is created to visualize the survival percentages for different values of 'SibSp' (number of siblings/spouses aboard).

4. Mean Age by Embarked: A bar plot is created to show the mean age of passengers for each 'Embarked' category as percentages.
