# Loan Status Prediction

This project aims to predict the loan status of applicants based on various features using machine learning models. The dataset contains demographic and financial information about the applicants.

There are 2 csv's which are application.csv and credit_record.csv and then merged in the single csv called final_dataset.csv using excel 
Duplicate values are find in the application.csv around 348472 records there are multiple applicant's by the same customer, after removing the duplicate values end up having 90085 records.

Visualizations are performed using tableau platform
	• Male and female distribution
	• Own car distribution
	• Own property distribution
	• Education type distribution
	• Relationship status distribution
	• Housing type
	• Income type
	• Occupation type
	• Overdue status distribution
	• Total income distributions
	• Children count
	• Family count
	• Loan Vs. gender
	• Status Vs. Income type
	• Status Vs. gender
Certainly! Here's a structured explanation of the steps you took in your project. This can be used for a README file on Kaggle and for adding to your CV.

## Introduction
The objective of this project is to build a predictive model that accurately determines the loan status of applicants. This can help financial institutions in making better lending decisions.

## Dataset
The dataset contains 36,105 rows and 20 columns with information on demographics, financial status, and loan details. The features include:
- ID
- Gender
- Ownership of car and property
- Number of children
- Total income
- Income type
- Education type
- Family status
- Housing type
- Age and employment duration in days
- Various flags for communication means
- Occupation type
- Number of family members
- Months balance
- Loan status

## Data Preprocessing
1. **Loading and Initial Exploration**: Loaded the dataset and performed initial exploration to understand the structure and content of the data.
2. **Data Cleaning**: Checked for and confirmed no null values in the dataset.
3. **Renaming Columns**: Renamed columns for better understanding and readability.
4. **Mapping Loan Status**: Mapped the loan status to more descriptive labels.

## Feature Engineering
1. **Encoding Categorical Variables**: Used LabelEncoder to convert categorical variables into numerical form.
2. **Dropping Irrelevant Columns**: Dropped columns that are not useful for modeling (e.g., ID, mobile, family members, and children).

## Modeling
1. **Splitting the Data**: Split the data into training and testing sets with a ratio of 80:20.
2. **Variance Inflation Factor (VIF) Calculation**: Calculated VIF to check for multicollinearity among features.
3. **Model Training**: Trained Decision Tree and Random Forest models on the training data.

## Evaluation
1. **Model Performance**: Evaluated the performance of the models using accuracy score, classification report, and confusion matrix.
2. **Cross-Validation**: Performed cross-validation to assess the generalizability of the models.

## Results
- **Decision Tree**: Achieved an accuracy of 1.0, indicating potential overfitting.
- **Random Forest**: Achieved an accuracy of approximately 0.9997, showing better generalization than the Decision Tree.
- **Feature Importance**: Identified the most important features influencing the loan status prediction.

## Conclusion
The project successfully developed a predictive model for loan status with high accuracy. The Random Forest model demonstrated robust performance and generalization. Further work could involve addressing potential overfitting and exploring more sophisticated feature engineering techniques.
