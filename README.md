# H1N1_Vaccine_Predictive_Modelling

1. Dataset
Data has been obtained from the National 2009 H1N1 Flu Survey (NHFS). The dataset contains around 26000 observations and 33 attributes. These attributes can be split into 3 categories- Socioeconomic background, Opinions on illness and vaccination and Behaviour.
The goal is to predict the likelihood of an individual taking H1N1 vaccine.
The raw dataset is present in training_set_features.csv while the clean dataset is present in clean_dataset.csv

2. Exploratory Data Analysis
Exploratory data analysis has been carried out on the dataset. Columns with more than 10000 missing values were dropped. In other columns, missing values were imputed using the mode of that attribute.  Mode was used in place of mean as most attributes in the dataset are categorical in nature. A correlation matrix was also plotted to understand the impact of each explanatory variable on the response variable. 
Steps for EDA are present in flu_eda.ipynb

3. Modelling
- The following models were used for baseline modeling-Logistic Regression, Gradient Boosting, Gaussian Naive Bayes, Decision Tree, Random Forest.
- Five-fold cross validation was carried out and the accuracy of all the five models was computed.
- Next, the same models were trained taking into account only the top six explanatory variables
- Feature selection and hyperparameter tuning was carried out for both Logistic Regression and Gradient Boosting algorithms.
