# Forecasting Dow Jones Index Volatility during the COVID-19 crisis.

## Abstract
The paper has shown a clear improvement in near-term forecasting performance by adding appropriate Google Trends time series as predictors, in particular during recessions. While the paper was focused on economic indicators, we would like to tackle the stock market and especially the NASDAQ index (subject to change for an individual stock). Our goal will be to to relate the index volatility to the query volume of related search terms during the COVID-19 pandemic. To do so, we will first need to find the most relevant search terms for the selected index/stock. Then, we will use an AR model with and without Trends data to forecast the index/stock volatility. Finally, we’ll try to improve this model.

## Research questions
- How can we select the most relevant search terms?
- How much does adding Trends data outperform models not using it?
- What models perform the best when it comes to forecasting stock volatility?

## Proposed datasets
- DJI Index ( [yfinance](https://pypi.org/project/yfinance/) )
- Google Trends (of course…)

## Methods
- Data collection: Extract the index/stock time series for 2020 (until end of november) from Yahoo and (naively) the related search term queries from Google Trends.
- Models: Build a simple AR model for forecasting and try different ways to improve the search terms selection and dimensionality (PCA…)
- Analysis & improvement: We will analyze our model performance according to the following metric: Does adding Trends data improve the MSE?

## Reference for inspiration
"Quantifying Trading Behavior in Financial Markets Using Google Trends", Tobias Preis, Helen Susannah Moat & H. Eugene Stanley, 2013

## Questions for TAs (optional)
