# Cryptocurrencies

## Overview

This analysis creates a report that includes what cryptocurrencies are on the trading market and how they could go grouped to create classification system. This analysis uses __unsupervised learning__ , so there is no known output. For that it preprocesses data to fit the machine learning models . To group cryptocurrencies , it uses clustering algorithms, reduces components using __PCA__ and uses the data visualizations. 

## Results 

* Preprocessing Data for PCA

    The data has been preprocessed keeping all cryptocurrencies that are being traded, drpping __ISTrading__ column, dropiing rows that have at least one __NULL__         values     and having rows where coins have mined. Also, __CoinName__ column has been removed, __get_dummies()__ method converts text features in numbers and           standardized the       features using __StandardScaler__ . 
    
* Reducing Data Dimensions Using PCA

    Here we are reducing dimensions to three principal components, PC 1, PC 2  and PC 3.

* Clustering Cryptocurrencies using K-Means

    Here, an elbow curve has been created using __hvPlot__ to find the best value for K, in this analysis, K is 4.  K-means algorithm makes preditions of the K (4)         clusters for cryptocurrencies’ data. 
    
    ![elbowcurve](https://user-images.githubusercontent.com/107717882/196512050-b5410a6c-c937-42e1-a6bb-a722c98e7189.png)

    
* Visualizing Cryptocurrencies Results 

    Using scatter plots with Plotly Express and hvPlot, the distinct group that corresponds to the three principal components are visualized. 
    
    ![3dpattern](https://user-images.githubusercontent.com/107717882/196512084-27a3f8c9-e1b0-4895-9de1-78d28d504e6c.png)

    ![hvPlot](https://user-images.githubusercontent.com/107717882/196512108-3f73705c-6148-4ae8-b502-71e9dca2e5d0.png)

    

## Summary

Unsupervised machine learning finds all kinds of unknown patterns in data. Using unsupervised algorithms we can find features that help categorize data. These      algorithms discover hidden patterns or data groupings .  Here, the pattern has been found using three main components. Visualization shows that pattern and classifications. That will help clients who are preparing to get into cryptocurrency market. 
