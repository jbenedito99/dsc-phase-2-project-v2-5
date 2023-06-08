# Overview

This repository contains documents for a project, which entailed the multiple linear regression analysis of a dataset housing information on houses in King County. The main features of the repository are a presentation, a file detailing the various columns of the dataset, and the dataset itself. 

# Business Context 

Generally-speaking, this repository is applicable to people looking to renovate their homes before selling them. In particular, the target audience are clients that want to increase their house's market value. In terms of the specific stakeholders for this project, the theoretical clients were residents in King County who wanted to increase the sale price of their homes to <b>at least $1M</b> by performing renovations on different features. 

The business question this project aimed to answer was: 
* <b>What combination of house features predict its sale price best?</b> 

# The Dataset

The dataset used for the project was the <b>kc_house.csv</b>. It has <b>25 columns</b> and over <b>30,000 entries</b>. The main columns of interest were: 
   
* `sqft_living`
* `grade/rating`
* `bathrooms`
* `price`

<b>Price</b> was used as the dependent variable, while <b>sqft_living</b>, <b>grade/rating</b>, and <b>bathrooms</b> were used as the independent variables in the final linear regression model. 

# Modeling and Regression Results

Here is a print out of the final linear regression model summary: 

![image](https://github.com/jbenedito99/dsc-phase-2-project-v2-5/assets/125815448/abe7edb3-7fec-4653-ba79-4129047a6d73)

The <b>adjusted R-squared</b> value says that <b>43% of the variation in price</b> is accounted for by the model. 

In terms of the model coefficients:
* Each unit increase in <b>sqft_living</b> led to an <b>increase in price</b> of <b>about 0.02%</b>. 
* Increasing <b>grade/rating</b> led to an <b>increase in price</b>. (Ex: an increase from 7 to 8 increases price by about 16%) 
* Each <b>additional half-bathroom</b> led to an <b>increase in price</b> of <b>about 1.43%</b>.

# Conclusion

My suggestions are:
* Increase <b>sqft_living</b> to <b>at least 2000 square feet</b>
* Have a <b>grade/rating</b> of <b>8 or higher</b>
* Have <b>at least 2.5 bathrooms</b>

# Sources and References 

* [Presentation](https://docs.google.com/presentation/d/1AcLuoKZqeQZ_nKB6Mj50B9WjmHtHx0_HMjpkTYuMeJc/edit?usp=sharing) 
* Used code from [this source](https://github.com/mojo-flat/Linear-Regression-GP-2) to transform categorical variables. 
* Used code from [this source](https://medium.com/analytics-vidhya/predicting-king-county-house-prices-with-multiple-linear-regression-84de5feeafb2) to get rid of outliers in dataset. 
