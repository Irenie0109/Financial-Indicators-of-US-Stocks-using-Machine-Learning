# Financial-Indicators-of-US-Stocks-using-Machine-Learning
# Reference : https://www.kaggle.com/datasets/cnic92/200-financial-indicators-of-us-stocks-20142018
# Dataset Insights
"""
Financial Indicators of US stocks - contains 4 dataset of financial indicators of each year from 2014 to 2018.Each dataset contains 200+ financial indicators, that are commonly found in the 10-K filings each publicly traded company releases yearly, for a plethora of US stocks (on average, 4k stocks are listed in each dataset).

There are still some important remarks within the=ose datasets:
Some financial indicator values are missing (nan cells), so the user can select the best technique to clean each dataset (dropna, fillna, etc.).

There are outliers, meaning extreme values that are probably caused by mistypings. Also in this case, the user can choose how to clean each dataset (have a look at the 1% - 99% percentile values).

The third-to-last column, Sector, lists the sector of each stock. Indeed, in the US stock market each company is part of a sector that classifies it in a macro-area. Since all the sectors have been collected (Basic Materials, Communication Services, Consumer Cyclical, Consumer Defensive, Energy, Financial Services, Healthcare, Industrial, Real Estate, Technology and Utilities), the user has the option to perform per-sector analyses and comparisons.

The second-to-last column, PRICE VAR [%], lists the percent price variation of each stock for the year. For example, if we consider the dataset 2015_Financial_Data.csv, we will have:

200+ financial indicators for the year 2015;
percent price variation for the year 2016 (meaning from the first trading day on Jan 2016 to the last trading day on Dec 2016).
The last column, class, lists a binary classification for each stock, where

for each stock, if the PRICE VAR [%] value is positive, class = 1. From a trading perspective, the 1 identifies those stocks that an hypothetical trader should BUY at the start of the year and sell at the end of the year for a profit.
for each stock, if the PRICE VAR [%] value is negative, class = 0. From a trading perspective, the 0 identifies those stocks that an hypothetical trader should NOT BUY, since their value will decrease, meaning a loss of capital.
The columns PRICE VAR [%] and class make possible to use the datasets for both classification and regression tasks:

If the user wishes to train a machine learning model so that it learns to classify those stocks that in buy-worthy and not buy-worthy, it is possible to get the targets from the class column;
If the user wishes to train a machine learning model so that it learns to predict the future value of a stock, it is possible to get the targets from the PRICE VAR [%] column
"""
# Machine Learning Purpose
"""
After completing this Machine Learning project, Irene expects to find out the best Models for the dataset to predict the decision whether we should invest on the specific stocks based on different indicators. Because the datasets are labelled, so that within this project, Irene has applied Supervised Learning which discovers patterns from the datasets and builds a model that can be used in a new dataset
"""
