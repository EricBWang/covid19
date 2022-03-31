# Exploring COVID-19 Point Prevalence
COVID-19 Point Prevalence is a linear model project aimed at providing insights on how COVID-19 spreads, identifying areas of vulnerability, and guiding policy or medical decisions by utilizing core ideas of data science principles and techniques. 

Results
* An ordinary least squares model involving social vulnerability (medicare enrollment) and health risk factors (i.e. diabetes, heart disease, smokers) obtained the lowest MSE across train/test splits, signaling that these features are worth exploring further
* Identified significant correlations between health risk groups and COVID-19 susceptibility via correlation heatmaps, suggesting the significance of comorbidities in understanding the virus
* Determined that many demographic features, including population density, were less effective than initially hypothesized

Procedure
* Constructed our data, consisting of demographic, health risk, and social distancing factors by merging time-series datasets of county-level features, confirmed cases, and confirmed deaths after data cleaning 
* Confirmed cases divided by population was selected as a metric for point prevalence
* Created choropleth of COVID-19 confirmed cases by county, correlation heat maps, and pairwise scatter plots with logarithmic transformations for various features
* Utilized scikit-learn’s cross validation functions alongside train-test splits, regularization, and hyperparameter tuning
* Assuming homoscedasticity and errors with mean zero, compared an ordinary least squares, lasso regression, and ridge regression model based on their respective mean squared error loss functions 

