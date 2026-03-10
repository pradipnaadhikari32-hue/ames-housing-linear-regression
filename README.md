House Price Prediction

A machine learning project that predicts residential house sale prices using Linear Regression on the Ames Housing dataset. Developed as the final project for the Foundation of Data Science Lab.

Overview

This project demonstrates the complete data science workflow, including problem definition, exploratory data analysis (EDA), model building, evaluation, and interpretation.

The goal is to predict the sale price of a house using features such as living area, overall quality, year built, and garage capacity.

Dataset

Ames Housing Dataset
Source: https://www.kaggle.com/datasets/prevek18/ames-housing-dataset

2,930 residential property records from Ames, Iowa

Around 80 numerical and categorical features

Target variable: SalePrice

Download the dataset from Kaggle and place the file AmesHousing.csv in the project directory.

Project Structure
house-price-prediction/

house_price_prediction.py   # Main project script
AmesHousing.csv             # Dataset (download separately)
eda_plots.png               # EDA visualizations (generated)
model_evaluation.png        # Actual vs predicted plots
feature_importance.png      # Feature coefficient chart
README.md
Methodology
Problem Definition

The task is to predict a continuous numeric variable (SalePrice). Linear Regression was chosen because it is simple, interpretable, and suitable for regression problems.

Data Collection

The project uses the Ames Housing dataset. Important features include:

Above-ground living area

Overall quality rating

Year built

Basement square footage

Garage capacity

Data Preprocessing and EDA

Removed columns with more than 40% missing values

Imputed remaining missing values

Explored feature distributions and correlations

Encoded categorical variables using Label Encoding

Applied Standard Scaling

Split data into 80% training and 20% testing sets

Model Building

Three regression models were trained and compared:

Model	Description
Linear Regression	Baseline regression model
Ridge Regression	Linear regression with L2 regularization
Lasso Regression	Linear regression with L1 regularization
Model Evaluation

Models were evaluated using:

R² Score – proportion of variance explained by the model

MSE (Mean Squared Error) – average squared prediction error

RMSE (Root Mean Squared Error) – error in dollar units

Interpretation and Conclusion

Feature coefficients from the Linear Regression model were analyzed to determine the most influential predictors.

Overall Quality and Above-Ground Living Area were the strongest predictors of house sale prices.

Requirements

Install required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn
Usage

Clone the repository:

git clone https://github.com/your-username/house-price-prediction.git
cd house-price-prediction

Download the dataset from Kaggle and place AmesHousing.csv in the project folder.

Run the script:

python house_price_prediction.py

The program will automatically generate visualization plots in the project directory.

Results

The Linear Regression model predicted house prices with reasonable accuracy.

Key observations:

Overall Quality and Living Area strongly influence sale price

Ridge and Lasso models produced similar performance to Linear Regression

RMSE represents the average prediction error in dollars

Author

Final project for the Foundation of Data Science Lab.

License

For academic use only.
