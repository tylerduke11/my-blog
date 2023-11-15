---
layout: post
title:  "Is NBA Player Performance Correlated with Player Salary?"
author: Tyler Duke
description: "An analysis of NBA players and their performance related to their salary"
date: Nov 14, 2023
image: ![coverimage](my-blog/assets/images/nba-banner.png)
--- 

## Introduction and Motivation
Have you ever wondered how NBA player performance is linked to their salary? Players make a lot of money but do the best players always get paid the most? I have always had this question in my mind because theoretically, the best players should be getting paid the most. After all, they are contributing the most to the team they are on. So, I decided to conduct an in-depth analysis of the data from the 2022-2023 NBA basketball season to determine if player performance is correlated with player salary. 

## Description of Data Collection and Cleaning
I used Python to scrape the data I was interested in for my analysis. I scraped player statistics from the [nba.com](https://www.nba.com/stats/players/traditional?Season=2022-23) website and player salaries from the [hoopshype.com](https://hoopshype.com/salaries/players/2022-2023/) website. I had to use a Selenium webdriver for the player statistics because the main page only displayed the first 50 rows of player data, but I wanted all the player data. I then used the BeautifulSoup library to scrape the data for all players in the 2022-2023 season. For the player salary website, I only had to use BeautifulSoup because the table was on the main page. I used a for loop on each link to grab all the html information I needed.

I then cleaned the data by eliminating some unnecessary rows I wasn't interested in for each table. Finally, I merged the data together to make one final data set that I will be using for analysis.

Here is a link to my [code](https://github.com/tylerduke11/Semester-Project-386/blob/main/basketball.py) and my [data](https://github.com/tylerduke11/Semester-Project-386/blob/main/nba_data.csv) in my GitHub repository.

## Ethical Considerations
Web scraping has the potential for ethical concerns if the correct measures are not taken. I made sure to check the robots.txt pages on each website I scraped to ensure that I was scraping legal information from the websites. 



## Conclusion
I hope you enjoyed this project as much as I have as we explored the relationship between NBA player performance and salary.
