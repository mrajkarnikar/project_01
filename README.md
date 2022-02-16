

# Project Title

Olympic Trend Analysis


# Project Description

In this project, we are tryig to analyze historical data of olympics and analyze different trends on the data. Some of questions we are trying to answer are:

1. Find trend for how highest number of  winner of medals by country have changed across the history
2. Find trend of top 5 sports where USA has won the most number of gold over the years
3. Find the relationshiop of population, gdp and medal count. Does more population and gdp mean more medal count ? 
4. Find trend on age of Male and Female Atheletics

# Team Members

- Chris Contos
- Manish Rajkarnikar
- Abdullahi Osman


# Data Description

We are using 2 sources of data 

### Kaggle
Using kaggle we were able to go to historical dataset[0] on the modern Olympic Games, including all the Games from Athens 1896 to Rio 2016.



### Worldbank
Worldbank DataBank[1] contains collections of time series data on a variety of topics on various countries. We can create our own queries; generate tables, charts, and maps; and easily save, embed, and share them. We use Worldbank DataBank API interface of to extract information such as population and gdp of various countries throughout the history



# How to run the project

In order to run the project, we should be able to run notebook named manish.ipynb and chris.ipynb  

We also have created a dashboard to put all the slides together. That code is in dashboard.ipynb

# Find trend for how highest number of  medal winners by country have changed across the history

kaggle[0] provides information of all the atheletics that participated in the olympics. It contains information such as their name, the country they are from, medal they won and the sport in which they won the medal in and also the year in the medal was won. Using this information we were able to find the number of medals each country won and rank the top twenty countries who won the most number of medal in each olympics. Using this information we were then able to plot the following animation to find a trend for how highest number of  winner of medals by country have changed across the history

![Myplot](./history.gif)



From the above chart we can conclude that USA did not use to be leader when the olypmics started.
* US started being dominant since the 1920s.
* Early competitors where countries like european countries like Sweden, Belgium, Italy, France .
* From 1950s Russia started being the competitor
* China started doing better since 2000

# Find trend of top 5 sports where USA has won the most number of gold over the years

We were able to tap into kaggle data[0] again to group number of medal won in various years  filtered it only for  USA. We wanted to see what were the top 5 sports where USA has won the most number of gold over the years. 

![top_5_winning_category_pie_chart](./top_5_winning_category_pie_chart.png)

![top_5_winning_category_usa](./top_5_winning_category_usa.png)


Above diagram show that overall US has been winning most of the medals in this order
1. Swimming
2. Atheletics 
3. Basketball
    
US used to win a lot in rowing also. Lately, we can see a trend that football is another sport where US has been getting a lot of medals from.


# Find the relationshiop between population, gdp and medal count. Does more population and gdp mean more medal count ? 

We were interested in finding if gdp and population of country have any effect on the number of medals won in olympics. In other words, we wanted to find the relationshiop of population, gdp and medal count. kaggle data[0] did not have any population or gdp information. So we can find another source for that data. We found that world bank API provided that data. But the data went as far back as 1971 only. We then took subset of data from kaggle and joined this information with world bank data and were able to plot a diagram below

![gdp_pop_medal_count_reln](./gdp_pop_medal_count_reln.png)

This diagram showed us  that small countries and small population usually mean less number of medals. But not necessary all the time. You can see that few countries like india and china(in the past) could not get many medal despite having larger population.  

# Find trend on age of Male and Female Atheletics

As for age trend, we see very consistent pattern where male and female age is around mid 20s throughout the history.

![male_age_trend](./male_age_trend.png)

![female_age_trend](./female_age_trend.png)



[0] https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results

[1] https://databank.worldbank.org/indicator/NY.GDP.MKTP.CD/1ff4a498/Popular-Indicators