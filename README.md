# Project-1
Title:Has COVID deaths affected happiness scores.

Contributors: Parker Teske, Carie Bates, Francisco Martinez, Victoria O’Byrne, Katharyn Hogle, Corey Monsma

Outline: Using data from the world happiness reports from  2015 to 2022  we will determine which Countries offer the highest happiness score, we will focus on the top 20 countries to determine how much the happiness score is affected by GDP and life expectancy .  Using regression analysis we will determine if the scores are positively or negatively impacted by COVID mortality rates in 2020-2022. This analysis can be used by the healthcare industry.

Data source: Happiness scores are from the World Happiness report 
World Happiness Report up to 2022 | Kaggle - happiness data, the happiness score is determined by six factors; levels of GDP, life expectancy, generosity, social support, freedom, and corruption)
COVID mortality rates are from John Hopkins Medical.
Life expectancy data from World Bank.


Null Hypothesis:
Happiness scores were not impacted by by covid deaths in the years 2020 through 2022.
Alternative Hypothesis:
Happiness scores were negatively impacted by covid deaths in the years 2020 through 2022 with a confidence level of 95% or p value < .05.

Data Analysis:
Happiness_CovidDeaths-Presentation.ipynb

csv files are imported 
pandas dataframes are created
Data is merged for happiness and covid datasets for 2020, 2021, 2022, data is merged on 'Country Name'
merged_data_2020 = pd.merge(csv2020df, time2020df, how='left', on = ['Country name'])
merged_data_2021 = pd.merge(csv2021df, time2021df, how='left', on = ['Country name'])
merged_data_2022 = pd.merge(csv2022df, time2022df, how='left', on = ['Country name'])

Happiness mean and COVID death mean calculated for years 2018-2022

Data for 2020, 2021, 2022 is plotted to a scatter plot

Ttest_indResult(statistic=-2.302773775704768, pvalue=0.02221680343150734)
We can reject the Null Hypothesis, since the p value is < 0.05
Over the years from 2018 to 2022, we can see that both the averages of happiness scores and the average covid deaths around the world rose. We performed an Independent T-Test comparing the happiness scores of all the countries in 2018 with the scores from 2022 which resulted in a p-value of 0.0222. With this p-value, we reject the Null Hypothesis because the increase in happiness scores between 2018 and 2022 was not random. We also showed the United States' happiness scores and covid deaths across 2018 – 2022 to visualize a single country’s growth path in those two areas.
Using a line graph, we were able to see how the average happiness scores rose seemingly disconnected from the path of the average life expectancy. However, when we broke it down into the years 2018, 2020, and 2022 and compared Life Expectancy with Happiness Scores we were able to see a positive correlation. 2018 r-value: 0.642411, correlation value: 0.8 2020 r-value: 0.611112, correlation value: 0.78 2022 r-value: 0.551364, correlation value: 0.74












