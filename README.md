# Titanic Data Preprocessing

This project demonstrates data cleaning and preprocessing using the Titanic dataset. It is designed as part of an internship task to practice essential data preparation techniques for machine learning.

## Dataset

Dataset used: Titanic dataset from Kaggle  
Link: https://www.kaggle.com/datasets/yasserh/titanic-dataset

Ensure that the file `train.csv` is placed in the same directory as the script before running it.

## Steps Performed

1. Load and Explore Data  
   - Loaded the dataset using pandas  
   - Displayed data overview using info and describe functions

2. Handle Missing Values  
   - Imputed missing values in the 'Age' and 'Fare' columns using mean  
   - Filled missing 'Embarked' values using the most frequent value (mode)

3. Encode Categorical Variables  
   - Converted 'Sex' and 'Embarked' columns to numerical format using LabelEncoder

4. Feature Engineering  
   - Created 'FamilySize' by combining 'SibSp' and 'Parch'  
   - Created 'IsAlone' to indicate if the passenger was traveling alone

5. Outlier Removal  
   - Applied the Interquartile Range (IQR) method to remove outliers from the 'Fare' column

6. Normalize Features  
   - Scaled 'Age', 'Fare', and 'FamilySize' using StandardScaler

7. Data Visualization  
   - Created a boxplot to visualize Age distribution based on survival  
   - Created a heatmap to show feature correlations

## Tools and Libraries Used

- pandas  
- numpy  
- seaborn  
- matplotlib  
- sklearn (SimpleImputer, LabelEncoder, StandardScaler)

## Output

The script displays key visualizations and prepares a cleaned dataset ready for model training.

## How to Run

1. Ensure all required libraries are installed  
2. Place the Titanic dataset (`train.csv`) in the working directory  
3. Run the script using any Python environment

