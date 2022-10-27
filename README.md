# IMDB Movies Analysis
This is a project from scratch starting by scraping the data then cleaning and analyzing it.

## Project Overview
* The aim of this project is to extract interesting insights from the top 200 IMDB movies.
* The dataset used has been scraped using the BeatifulSoup Library and saved as a csv file.
* Extensive cleaning has been carried out on the data producing a well formatted and ready to analyze data.
* Comprehensive analysis has been done using the cleaned data. Different visuals has been utilized to ensure intuitive results.

## Code and Resources Used
* Dataset: Data has been scraped from https://www.imdb.com/search/title/?count=100&groups=top_1000&sort=user_rating
* Python Version: 3.9
* Packages: 
    - Pandas:provides data analysis/manipulation tools
    - Numpy: fundamental package for scientific computing in Python.
    - Matplotlib: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.
    - Seaborn: based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.
    - bs4 (BeautifulSoup version 4 used to pull data out of HTML and XML files).
    - urllib (opening and reading URLs)
    - googletrans: A Python library that implemented Google Translate API.
* Scraping: [Web scraping in Python with Beautiful Soup and requests from Data School](https://www.youtube.com/playlist?list=PL5-da3qGB5IDbOi0g5WFh1YPDNzXw4LNL)
* Cleaning: https://stackoverflow.com/questions/13445241/replacing-blank-values-white-space-with-nan-in-pandas
* Investigating association among categorical features: https://towardsdatascience.com/the-search-for-categorical-correlation-a1cf7f1888c9
* Model selection automation: https://www.youtube.com/watch?v=7uLzGRlXXDw
* For Web Framework Requirements: pip install -r requirements.txt
* Flask Productionization: https://towardsdatascience.com/productionize-a-machine-learning-model-with-flask-and-heroku-8201260503d2

## Data Cleaning
In this section we loaded the data from the .csv file into a Pandas DataFrame. We first changed the <code>TotalCharges</code> column from <code>string</code> to <code>float</code>. Then we dropped all null values and also the <code>customerID</code> column.

## EDA
EDA summary
## Model Building
First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.

I tried three different models:

* Multiple Linear Regression – Baseline for the model
* Lasso Regression – Because of the sparse data from the many categorical variables, I thought a normalized regression like lasso would be effective.
* Random Forest – Again, with the sparsity associated with the data, I thought that this would be a good fit.

## Model performance

The Random Forest model far outperformed the other approaches on the test and validation sets.

* Random Forest : MAE = 
* Linear Regression: MAE = 
* Ridge Regression: MAE = 

## Model Deployment
