# Project-1
Title:Where should we move to ?

Contributors: Parker Teske, Carie Bates, Francisco Martinez, Victoria O’Byrne, Katharyn Hogle, Corey Monsma

Outline: Using data from the world happiness reports from  2015 to 2022  we will determine which Countries offer the highest happiness score, we will focus on the top 20 countries to determine how much the happiness score is affected by GDP and life expectancy .  Using regression analysis we will determine if the scores are positively or negatively by COVID mortality rates in 2020-2022. This analysis can be used by the healthcare industry.

Data source: Happiness scores are from the World Happiness report 
World Happiness Report up to 2022 | Kaggle - happiness data, the happiness score is determined by six factors; levels of GDP, life expectancy, generosity, social support, freedom, and corruption)
COVID mortality rates are from https://covid19.who.int/WHO-COVID-19-global-data.csv


Null Hypothesis:
Happiness scores were not impacted by by covid deaths in the years 2020 through 2022.
Alternative Hypothesis:
Happiness scores were negatively impacted by covid deaths in the years 2020 through 2022 with a confidence level of 95% or p value < .05.


csv files are imported 
pandas dataframes are created
Data is merged for happiness and covid datasets for 2020, 2021, 2022, data is merged on 'Country Name'

Happiness average and COVID death average calculated for years 2018-2022






