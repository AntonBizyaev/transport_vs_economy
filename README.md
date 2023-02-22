# How Transport Tnfrastructure Deficit Can Affect Economic Development

Theoretical research suggests that transport infrastructure is a necessary condition for economic development, i.e. transport infrastructure deficit might hinder economic growth by creating a bottleneck effect. 

However, there is a gap in empirical understanding of this phenomenon, especially under international comparison.

**Note**: *This analysis is part of my research article: Bizyaev A. Transport infrastructure deficit and economic development: Israeli case. Finance and Business. St. Petersburg. 2021. In Russian.*  

*The code I use here is a Python adaptation of my original code written in R.*

## Problem

We need to investigate relationship between transport infrastructure and economic development using data analysis tools.

## Data

The data is present for 27 countries, has 17 variables and covers three time periods: 1995, 2005 and 2015.

The dataset has already been preprocessed for the purposes of research: every variable (whenever applicable) has been converted either into per capita terms or into percentages to allow for international comparison.

## Analysis

1. Apply PCA to "compress" all 17 variables into 2, i.e. transport and economy
2. Use cluster analysis (k-means) to split the countries into different groups and study their behavior separately
3. Estimate the direction of relationship between transport and economy within clusters using linear regression
4. Track clusters' evolution by comparing the results across three time periods

## Results

The above analysis has shown that different groups of countries exhibit different relationship between transport infrastructure level and economic development: 

* In countries with relatively developed economies but low levels of transport infrastructure supply (e.g. Western Europe), the deficit of the latter is hindering economic growth. Some of these countries are losing in traffic jams up to 6% of their GDP annualy.
* Countries with low levels of both economic and trasnport indicators (e.g. Balcan countries) have not shown consistent relationship between the former and the latter
* Countries with relatively high supply of transport infrastructure but low levels of economic development (e.g. Baltic and Eastern European countries), and countries with high levels of both indicators (e.g. Scandinavian countries) have demonstrated a negative relationship between economy and transport infrastructure.

Each case has been provided with a possible theoretical explanation. Nevertheless, a deeper inquery into economic history and transportation market conditions of every country group can be a fruitful line for future research.

## Links
**Code:** <a href='https://github.com/AntonBizyaev/transport_vs_economy/blob/main/transport_vs_economy.ipynb'>jupyter notebook</a>  
**Data:** <a href='https://github.com/AntonBizyaev/transport_vs_economy/blob/main/data.xlsx'>source</a>  
**My original article (in Russian):** <a href='http://finbiz.spb.ru/wp-content/uploads/2021/05/bisaev_1_2021.pdf'>article</a>

