# FORCASTING GDP USING ECONOMIC INDICATORS

Tableau Dashboard: [Link to Dashboard](https://public.tableau.com/shared/YXW5QSG39?:display_count=n&:origin=viz_share_link)
[Overview](https://public.tableau.com/authoring/MajorTrendsBetweenDevelopingVsDevelopedCountries/FORECASTINGGDP#1)

## Overview:
The team has decided to create a predictive Machine Learning model to forecast nominal GDP (GDP current in USD). We used country data retrieved from the World Bank, spanning from 1961 to 2021. Variables impacting GDP, include, but are not limited to, macroeconomic and socio-economic variables, such as inflation, unemployment rate, urbanization rate, energy use and consumption, education levels and health expenditure. We performed ETL on a dataset of nearly 175,000 observations. Then we ran 2 machine learning models for developing and devoped countries. We visualized the data in Tableau. Finally, we were able to understand the most impactful factors to economic growth. 


## Tools:
Python for (ETL)
Jupyter notebook
Machine Learning
Tableau

## Model:
We tested the following models on our dataset:

1. Linear Regressor Model (with and without scaling)
2. Random Forest Regressor Model
3. Support Vector Regressor Model(with different Kernels)

## ETL:
* We read in the CSV file and drop unnecessary columns;
* We remove special unwanted characters that represented missing data, we replace them with naan values;
* We filter out country groups (Africa, Europe, etc.) and leave in the individual countries only;
* We drop the years that have more than 70% of data missing;
* We convert the data into float (as Python reads it as object);
* We fill in missing row values with row averages;
* We convert the data from wide to long format, with years as a single column and each variable as a column;
* We remove outliers using IQR;
* After performing ETL, we filtered countries into two categories (developed and developing) countries(based on gdp/per capita). We use the Investopedia definition of a developed country: A country with a GDP per capita over $12,000 is defined as developed. Countries with a GDP per capita less than $12K is defined as developping.
Will be running 2 machines learning models, predicting GDP over using socio-economic indicators(2019-2023);

## Machine Learning:
We performed a variety of models including Unsupervised Machine Learning, but found the best accuracy with regression in the form of the Random Forest model.

## Visualizations:
1. How GDP affected CPI.
2. How all economic indicators responsed in developed and developing countries.
3. Bar charts showing Urbanization, Unemployment and Life Expectancy in G7 countries.
4. Map illustrations showing countries based on gdp per capita and inflation.

## Results:
Based on data set (1961-2021) we will be presenting the following outcomes:
Random Forest Model.

![image](https://user-images.githubusercontent.com/111619125/217625873-25535846-ebae-485b-81be-8d94e7c46069.png)


## Summary:
A comparative and visually descriptive dataset comparing developing countries and their economies. This dataset will utilize information gathered from WHO's website and include an ERD diagram and content produced using aspects of Machine-Learning, Tableau, Python, Jupyter notebook and Pandas libraries.
