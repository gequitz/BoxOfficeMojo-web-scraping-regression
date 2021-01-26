# BoxOfficeMojo-web-scraping-regression
Metis Project 2: Linear Regression

By: Gabriel Equitz
______________________________________________________

## Problem Statement
- Our goal is to help movie companies efficently allocate resources to profit from their multimillion dollar expenses. Over 80% of Hollywood movies fail to turn a profit
- The target variable = worldwide box office gross
- Features include: Distributor (studio), Budget (USD), Foreign Market Count, Genres (10), and Rating (MPAA)
- We choose to analyze box office data from the Top 200 Lifetime Grossing movies of all time
- The project findings will be compiled and presented in Google Slides

## Data Sources
- [https://www.boxofficemojo.com/chart/ww_top_lifetime_gross/?area=XWW&ref_=bo_cso_ac](BoxOfficeMojo_top_worldwide_grossing_films)

## Methodology
- Get the relevant datasets by webscraping BoxOfficeMojo
- Choose appropriate items for exploratory data analysis
- Data cleaning, save the webscraped file as .csv
- Linear regression
- Analyze features correlated with our project goals (budget, rating, etc.) - Find the highest R^2
- Create data visualizations
- Presentation preparations (Google Slides)

## Findings- 
- Foreign market count was positively correlated
- Adventure had the highest R^2 = 0.035, Crime had the lowest R^2 = 0.0004 (both positively correlated)
- Disney had highest R^2 out of all distributors
- Higher budgets correlated with higher box office gross. R^2 = 0.215
- PG-13 provided the greatest R^2 out of ratings
- LASSO provided the best results, with R^2 = 0.3327, MAE = $42.8 million 

## Libraries and Notebook used
- [Jupyter Notebook](https://jupyter.org/)
- [Pandas](https://pandas.pydata.org/)
- [Numpy](https://numpy.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Seaborn](https://seaborn.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [LXML](https://lxml.de/)

## Blog link
- TBD
