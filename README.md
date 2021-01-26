# BoxOfficeMojo-web-scraping-regression
Metis Project 2: Linear Regression

By: Gabriel Equitz
______________________________________________________

## Problem Statement
- Our goal is to help movie companies efficently allocate resources to profit from their multimillion dollar expenses. Over 80% of Hollywood movies fail to turn a profit
- The target variable = box office gross
- Features include: Distributor (studio), Budget (USD), Foreign Market Count, Genres (10)
- We choose to analyze box office data from the Top 200 Lifetime Grossing movies of all time
- The project findings will be compiled and presented in Google Slides

## Data Sources
- https://www.boxofficemojo.com/chart/ww_top_lifetime_gross/?area=XWW&ref_=bo_cso_ac (BoxOfficeMojo)

## Methodology
- Get the relevant datasets by webscraping BoxOfficeMojo
- Choose appropriate items for exploratory data analysis
- Data cleaning, save the webscraped file as .csv
- Linear regression
- Analyze features correlated with our project goals (budget, rating, etc.) - Find the highest R^2
- Create data visualizations
- Feature data was scraped from pages on BoxOfficeMojo.com, and parsed HTML after- To find the highest R^2, linear regression was used w
- Presentation preparations (Google Slides)

## Findings- 
- Foreign markets was positively correlated with R^2 = 0.0527
- Adventure had the highest R^2 = 0.035, Crime had the lowest R^2 = 0.0004
- Higher budgets correlated with higher box office gross

- LASSO provided the best results, with R^2 = 0.24, MAE = $35 M, MRE = 

## Libraries and Notebook used
- [Jupyter Notebook](https://jupyter.org/)
- [Pandas](https://pandas.pydata.org/)
- [Numpy](https://numpy.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Matplotlib](https://matplotlib.org/)- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)- [LXML](https://lxml.de/)
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
- [LXML](https://lxml.de/)
- [Seaborn](https://seaborn.pydata.org/)

## Blog link
- TBD
