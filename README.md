# Summary of Melbourne Housing Analysis in R

This project presents a statistical analysis of housing prices in Melbourne, Australia using R.

The goal is to identify key factors that influence property prices and provide insights that help those who want to buy a good deal house.

#### Note
This README contains only the summary. For the full analysis, code, and detailed explanations, please refer to the code_report file.

## Purpose
Melbourne is one of the most popular cities in the world, so the housing prices are getting high because of its high demand. 

In this project, I applied the statistical knowledge acquired in my coursework to a real-world problem:

**What factors most strongly affect housing prices in Melbourne, and how can we identify good deals?**


## Data
I colleceted dataset from Kaggle. 

[url:https://www.kaggle.com/datasets/dansbecker/melbourne-housingsnapshot]

- Originally scraped from Domain.com.au by Tony Pino (2017)
Variables include:
- Address
- Type of real estate
- Suburb, Method of Sale
- Number of Rooms, Price
- Real Estate Agent
- Date of Sale
- Distance from the Central Business District (CBD).

## Method
I approached this analysis using statistical methods rather than complex machine learning techniques for my understand of fundational concepts.

#### Steps:
1. Data Cleaning & Preprocessing
2. Applied MLR and Checked residuals for Normality and the constant variance
3. Selected predictors based on AIC, BIC, and adjusted$R^2$
4. Applied GAM and Checked the linear and non-linear relationships between `Price` and predictors
5. One-way Anova for checking mean difference in `house type` and `room` columns
6. Two-way Anova for the interactions between `house type` and `room`


## Finding
The features of expensive properties in Melbourne are below:

- Number of rooms: more rooms correlate with hihger prices
- Property Type: houses, cottages, villas, semis, or terraces
- Year: newer properties are more expensive
- Lattitude: -37.9 and -37.8
- Longtitude: 144.9 and 145.1
- Landsize: around 800 $[m^2]$

Therefore, I can conclude that you should pay close attention to six key features: the number of rooms, the type of property, the old of houses, the location (latitude and longitude), and the land size. If a property has strong values in these features but is priced low, it might be undervalued and could represent a good buying opportunity.
