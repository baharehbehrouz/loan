# Loan Project

This project aims to predict the loan status of applicants based on their personal and financial information. The project uses Python and several libraries such as pandas, numpy, matplotlib, seaborn, and sklearn.

## Data

The data used for this project is the loan.csv file, which contains the data of 614 loan applicants with 13 features each. The features include the gender, marital status, education, employment status, income, loan amount, loan term, credit history, property area, and loan status. The loan status is the target variable that indicates whether the loan was approved or not.

The data is loaded and explored using pandas and matplotlib. The number and types of categorical variables are printed. The loan ID column is dropped as it is not relevant for the analysis. The categorical variables are encoded using a label encoder. The distribution of the categorical variables are shown using bar plots. The correlation matrix of the numerical variables are shown using a heatmap. A catplot is used to show the relationship between the gender, marital status, and loan status variables.

## Preprocessing

The data is split into features (X) and target (y) variables. The features are all the columns except the loan status column. The target is the loan status column.

The missing values in the data are imputed using the mean of each column. The data is then split into training and testing sets, with 80% of the data for training and 20% for testing. The random_state parameter is set to 42 to ensure reproducibility of the results.

## Model

The models used for this project are two different classifiers: K-Nearest Neighbors and Logistic Regression. These models are imported from the sklearn module and instantiated with the default parameters. The max_iter parameter is set to 10000 for the Logistic Regression model to avoid convergence warnings.

The models are fitted on the training data and used to make predictions on the training data. The accuracy of the models is evaluated by using the accuracy score, which measures the percentage of correct predictions. The accuracy scores for the training data are printed for each model.
