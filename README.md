# Oil and War

## Description

During this unfortunate period of war in Ukraine, we have noticed the daily rising price fluctuations in oil across the world, which made us ponder if we could predict the return and prices of oil in this current state of the world.
In this project, we aim to identify the periods of war and the sentiment of news articles around ‘petroleum’ to create a feature dataset along with the price of oil since 2000 until 2020 (specifically to ignore the pandemic aberration).

---
## Table of Contents
* [Description](#description)
* [Goals](#goals)
* [Technologies](#technologies)
* [Instructions](#instructions)
* [Conclusion](#conclusion)
* [Contributors](#contributors)
* [References and Resources](#references-and-resources)
* [License](#license)

---
## Goals 
Our goal is to compare two or more machine-learning models for identifying price and price direction of oil. For our predictions, we will use natural language processing to draw insights from news articles for the past 22 years. In addition, we will use oil close prices/returns, gold prices, S&P 500, as well as times of unrest (Iraq War 2003-2011). Machine learning typically requires extensive data preparation before the model can be trained. We will use Jupyter to prepare a training and testing dataset, and to train and compare the machine-learning model.
---
## Technologies
Our portfolio analysis will use the following technologies: 
* pandas
* numpy
* datetime
* pathlib
* nltk
* matplotlib
* analyzer
* dotenv
* New York Times API 
* yfinance API
* warnings
* tensorflow

---
[![forthebadge made-with-python](https://forthebadge.com/images/badges/made-with-python.svg)](https://www.python.org/) </br>
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try) </br>

## Instructions
1. To get the project started on your local machine, clone the GitHub repository. 
2. The first file we want to run is the [crude_news_data](crude_news_data.ipynb). This will get the New York Times API data for a set amount of years. *This may take around 45 minutes to run...*
3. The end result of this notebook will export a [combined_csv](combined_csv.csv) file in a headlines folder, with all other articles throughout each month. 
4. Next, we use the [crude_sentiments](crude_sentiments.ipynb) notebook that will get the news data from the [combined_csv](combined_csv.csv) and run a sentiment analysis which will export an [oil_sentiments](oil_sentiments.csv) csv file. 
5. Once we have the sentiment analysis data, we will load historical oil data and apply time series analysis and modeling to determine whether there is any predictable behavior in the [oil_sentiment_analysis](oil_sentiment_analysis.ipynb) notebook. 

## Conclusion
Predicting price using 2 of the regression models, and comparing the performance. 2nd predicting the direction of return using classification model and comapring the 2 classification models. 

---
### Questions

1. How has oil prices behaved in the past 22 years?
(GRAPH OF OIL PRICE)(GRAPH OF RETURN)

2. What is the sentiment of oil across the period based on news articles using NLP?
(SCREENSHOT OF ALL SCORES - MAYBE AS A PLOT INSTEAD OF DATAFRAME)

3. Identify other features for oil price movements (based on avialability of data)
(SCREENSHOT OF DATAFRAME HEAD USED - FEATURES)

4. Compare model performances with each other when predicting oil prices. 
(SCREENSHOT REGRESSION)

5. Compare model performances with each other when predicting oil returns direction. 
(SCREENSHOT CLASSIFICATION)

6. Compare feature importance in the movement of oil prices. 
(SCREENSHOT)

---

## Contributors
Our team: 
<h2><a href="https://github.com/GuilleMGN"><img src="https://avatars.githubusercontent.com/u/73862470?s=60&v=4" /> GuilleMGN</a></h2>

<h2><a href="https://github.com/ksmaria"><img src="https://avatars.githubusercontent.com/u/93277973?s=60&v=4" /> ksmaria</a></h2>

<h2><a href="https://github.com/Prabhdyals"><img src="https://avatars.githubusercontent.com/u/93745962?s=60&v=4" /> Prabhdyals</a></h2>

<h2><a href="https://github.com/Satheeshbm"><img src="https://avatars.githubusercontent.com/u/92489132?s=60&v=4" /> Satheeshbm</a></h2>

<h2><a href="https://github.com/Nitin-Thomas"><img src="https://avatars.githubusercontent.com/u/93697349?s=60&v=4" /> Nitin-Thomas</a></h2>

<h2><a href="https://github.com/dmerkulenko"><img src="https://avatars.githubusercontent.com/u/93617615?s=60&v=4" /> dmerkulenko</a></h2>

---
## References and Resources
[CNN Iraq War News](https://edition.cnn.com/2013/03/19/opinion/iraq-war-oil-juhasz/index.html ) <br />
[Yahoo Finance](https://ca.finance.yahoo.com/ ) <br />
[How to Collect Data From The New York Times Over Any Period of Time](https://towardsdatascience.com/collecting-data-from-the-new-york-times-over-any-period-of-time-3e365504004 ) <br />
[New York Times API](https://developer.nytimes.com/apis ) <br />

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Copyright © 2022