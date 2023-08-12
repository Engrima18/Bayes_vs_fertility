# Bayes_vs_fertility
Small project to test Bayesian analysis tools for studying determinants of fertility for adult males

## Brief introduction

In Italy, the issue of fertility is quite central in recent years, especially in the post-covid
period, there has even been talk of a recessionary phase in terms of birth rates. The underlying causes are many and particularly diverse. In addition purely socio-economic reasons and the crisis the country is experiencing in
this regard, another rather worrying trend was found to be strongly affecting the birth rate
in most Western countries: an analysis of 56 countries from 6 different continents recorded
a halving in sperm count from 1973 to 2018. The aim of our analysis is to study the main sources of infertility for a man. Given a
data set with a set of attributes deemed more or less informative, we choose to use a simple Bayesian logistic regression for the prediction of subject with normal or altered sperm
(analyzed according to the WHO (2010) criteria).
What we seek to highlight through this study is the relationship between bad habits, health
status, context (environment, social, and time of year), and fertility level.

## The data set

Let’s give a look to the first rows of the used data set from the [UCI repository](https://archive.ics.uci.edu/dataset/244/fertility):


<img width="485" alt="datas" src="https://github.com/Engrima18/Bayes_vs_fertility/assets/93355495/26f1f6dc-04d8-415e-8ffe-2386c4058c66">

Some plots for the Exploratory Data Analysis
|       |       | 
:-------------------------:|:-------------------------: 
<img width="485" alt="plot1" src="https://github.com/Engrima18/Bayes_vs_fertility/assets/93355495/ab5c59ed-e7b2-49e7-8cc2-27e7f6a5d857"> | <img width="485" alt="plot2" src="https://github.com/Engrima18/Bayes_vs_fertility/assets/93355495/6b373ce6-8071-4b4e-b8a0-122a0df237ab">

The study of correlations between features is also relevant to understanding the importance of certain predictors

<img width="485" alt="plot3" src="https://github.com/Engrima18/Bayes_vs_fertility/assets/93355495/4a4a17da-1953-46d7-a0bf-76e55e15a77b">

See the `report.pdf` file for a deeper analysis.

## The models 

In the `fertility.rmd` file you can find the bayesian analysis (complete of convergence analysis of the MCMC).
We used a **Bayesian Logistic Regression** and a **Probit  Regression** to predict the two classes of interest (normal vs altered sperm) and study the convergence of parameters for both models.

# Used technologies

![RStudio](https://img.shields.io/badge/RStudio-4285F4?style=for-the-badge&logo=rstudio&logoColor=white)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)

