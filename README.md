# IMDB Movies Analysis
This is a project from scratch starting by scraping the data then cleaning and analyzing it.

## Project Overview
* The aim of this project is to extract interesting insights from the top 200 IMDB movies.
* The dataset used has been scraped using the BeatifulSoup Library and saved as a csv file.
* Extensive cleaning has been carried out on the data producing a well formatted and ready to analyze data.
* Comprehensive analysis has been done using the cleaned data. Different visuals has been utilized to ensure intuitive results.

## Code and Resources Used
* Video tutoria: I loosely followed Ken Jee's playlist as a guide: [Data Science Project From Scratch](https://www.youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t)
* Dataset: Data has been scraped from [IMDb "Top 1000" (Sorted by IMDb Rating Descending)](https://www.imdb.com/search/title/?count=100&groups=top_1000&sort=user_rating)
* Python Version: 3.9
* Packages: 
    - Pandas:provides data analysis/manipulation tools
    - Numpy: fundamental package for scientific computing in Python.
    - Matplotlib: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.
    - Seaborn: based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.
    - bs4 (BeautifulSoup version 4 used to pull data out of HTML and XML files).
    - urllib (opening and reading URLs)
    - googletrans: A Python library that implemented Google Translate API.
* Scraping: [Web scraping in Python with Beautiful Soup and requests from Data School](https://www.youtube.com/playlist?list=PL5-da3qGB5IDbOi0g5WFh1YPDNzXw4LNL). This is the best video tutorial on the topic online.
* Max Hilsdorf has a medium article that helped so much doing the analysis in this projet especially anlyzing the lists within a           dataframes. It was the only source I could find in this topic. I really recommend checking out the full article from the link
  https://towardsdatascience.com/dealing-with-list-values-in-pandas-dataframes-a177e534f173

## Data Cleaning
In this section we loaded the data from the .csv file into a Pandas DataFrame. We first changed the <code>TotalCharges</code> column from <code>string</code> to <code>float</code>. Then we dropped all null values and also the <code>customerID</code> column.

## Analysis
EDA summary
