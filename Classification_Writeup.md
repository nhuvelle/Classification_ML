# Predicting fraudulent credit card transactions using Classificaiton
Nathan Huvelle

## Abstract
The goal of this project was to use classification models to predict whether a credit card transaction was legitimate or fraudulent, in order to help the credit card company flag certain transactions and avoid the costs of dealing with chargebacks. The data set was pulled from [Kaggle](http://kaggle.com). After EDA and modelling was performed on the dataset, the results were presented in a 5 minute video presentation to my classmates and instructers at Mets.

## Design
Since credit card transactions contain mostly private information, I created a ficticious company that was tasked with helping the credit card companies identify fraudulent transactions so they could intercept them before final settlement. Several classification models were trained and tested on the data. F1 score was the primary metric I focused on, but I tracked others as well. 

## Data
The dataset contained 284,207 rows each representing a distinct transaciton, although some duplicates were found and dropped from the set. There were 30 features, all numerical and all anonymous due to the privacy issues. 

## Algorithms
Logistic Regression and Random Forest were the 2 main classification models that I used on this dataset. Since the features were all nameless, and I had no prior domain knowledge in this subject matter, it was to decide on what type of feature engineering to do. I dropped a few features that seemed unimportant for logistic regression but for the most part I kept the features as is. 

*Model Evaluation and Selection*
A Random Forest model with 150 estimators, unbalanced class weights and max depth of 10 ended up giving the best performance. The best f1 score that was obtained was 0.83. 

##Tools
- Numpy, Pandas and statsmodels for EDA
- Scikit-learn for modeling 
- matplotlib and seaborn for visualisations
- Keynote for presentation slides

## Communication
The design and results of this project were discussed in a 5 minute video presentation accompanied by Keynote slides containing visuals and the key metrics. The presentation slides are attached in this repository.
