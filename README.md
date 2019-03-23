# Housing-Data-Analysis
Boston housing data is wrangled and analyzed to predict the house prices based on different features of the house using R. It also includes usage on machine learning models to predict the prices.

It is a group project as a part of MSIM coursework(Customer Analytics). The datset we used was downloaded from Kaggle and it has 79 explanatory variables which span across every detail of the house. Based on our the dataset and the problem we were trying to address, we came up with a customer-centric research question: _‘Which features of the Iowa Housing dataset influences the customer buying decision and how well can these features be used to predict future sale price of a house and attract potential house buyers’_
The goal of our research is to identify the factors that are most important to the buyers and which directly affects the sale price. Also, to create a regression model that is able to accurately estimate the price of the house given the features. The steps we followed are mentioned below:

    1. Data Preprocessing
    2. Exploratory Data Analysis
    3. Application of different machine learning algorithms
    4. Recommendations based on analysis/visualizations 
    
**Data Pre-processing:**  
The dataset consists of features in various formats. It has numerical data such as prices and numbers of bathrooms/bedrooms/living rooms, as well as categorical features such as zone classifications for sale, which can be ‘Agricultural’, ‘Residential High Density’, ‘Residential Low Density’, ‘Residential Low Density Park’, etc. Considering 79 variables were too many for our analysis, we wanted to reduce them and only include those which had the maximum correlation with the dependent variable - Sale Price. We *removed the NA/NULL* rows/columns in the data and also removed the features that had high muti-collinearity.

**Exploratory Data Analysis:**
We individually analyzed our dependent variable and all the important independent variables we considered using different plots to get a sense of their range, mean, median and other features. The independent variables we considered are Overall quality, External factors(Zoning Classification and Ground Living Area), Internal factors(Building type) and Aesthetic factors(Bathroom, Kitchen) along with the dependent variable saleprice.

**Machine learning models applied:**
We first normalized the data by applying logarithm and then built different models like linear regression, decision tree, random forest and other ensemble techniques(randomForest, adaboost). The code snippets for these models could be found in the files _BostonHousingData_analysis_2.Rmd and BostonHousingData_DT.Rmd_. We also predicted the prices of the houses using the models built and estimated its acuuracy. 


