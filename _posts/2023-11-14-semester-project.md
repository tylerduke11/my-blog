---
layout: post
title:  "Is NBA Player Performance Correlated with Player Salary?"
author: Tyler Duke
description: "An analysis of NBA players and their performance related to their salary"
date: Nov 14, 2023
image: "/assets/images/nba-banner.png"
--- 

## Introduction and Motivation
Have you ever wondered how NBA player performance is linked to their salary? Players make a lot of money but do the best players always get paid the most? I have always had this question in my mind because theoretically, the best players should be getting paid the most. After all, they are contributing the most to the team they are on. So, I decided to conduct an in-depth analysis of the data from the 2022-2023 NBA basketball season to determine if player performance is correlated with player salary. I will evaluate the "best" players through numerous metrics that are tracked by the NBA for each player. These metrics include: Age, GP (Games Played), FG% (Field Goal %), 3P% (3 Point %), FT% (Free Throw %), PTS (Points), REB (Rebounds), AST (Assists), DD2 (Double Doubles), TD3 (Trible Doubles), TW (Team Wins), and TL (Team Losses)

## Description of Data Collection and Cleaning
I used Python to scrape the data I was interested in for my analysis. I scraped player statistics from the [nba.com](https://www.nba.com/stats/players/traditional?Season=2022-23) website and player salaries from the [hoopshype.com](https://hoopshype.com/salaries/players/2022-2023/) website. I had to use a Selenium webdriver for the player statistics because the main page only displayed the first 50 rows of player data, but I wanted all the player data. I then used the BeautifulSoup library to scrape the data for all players in the 2022-2023 season. For the player salary website, I only had to use BeautifulSoup because the table was on the main page. I used a for loop on each link to grab all the html information I needed.

I then cleaned the data by eliminating some unnecessary columns I wasn't interested in for each table. I was most interested in the metrics I mentioned above, along with player information such as their name,  team, and Salary. Finally, I merged the data together to make one final data set that I will be using for analysis.


Here is an example of some of the final data set that I will be using for analysis:

|    | 	Player	                |  Team	| TW | TL | Age  | Salary     | PTS  |	GP   |	FG%  |	3P%  |	FT%  |	REB  |	AST | STL | BLK |  DD2  | TD3 |
|---:|-------------------------:|------:|---:|---:|-----:|-----------:|-----:|------:|------:|------:|------:|------:|-----:|-----|-----|-------|-----|
|0   |	Joel Embiid	            |  PHI	| 54 | 28 | 29.0 | 33616770.0 | 33.1 |	66.0 |	54.8 |	33.0 |	85.7 |	10.2 |	4.2 | 1.0 | 1.7	|  39.0 | 1.0 |
|1   |	Luka Doncic	            |  DAL	| 38 | 44 | 24.0 | 37096500.0 | 32.4 |	66.0 |	49.6 |	34.2 |	74.2 |	8.6  |	8.0 | 1.4 | 0.5	|  36.0 | 10.0|
|2   |	Damian Lillard	        |  POR	| 33 | 49 | 32.0 | 42492492.0 | 32.2 |	58.0 |	46.3 |	37.1 |	91.4 |	4.8  |	7.3 | 0.9 | 0.3	|  16.0 | 2.0 |
|3   |	Shai Gilgeous-Alexander |  OKC	| 40 | 42 | 24.0 | 30913750.0 | 31.4 |	68.0 |	51.0 |	34.5 |	90.5 |	4.8  |	5.5 | 1.6 | 1.0	|  3.0  | 0.0 |
|4   |	Giannis Antetokounmpo   |  MIL	| 58 | 24 | 28.0 | 42492492.0 | 31.1 |	63.0 |	55.3 |	27.5 |	64.5 |	11.8 |	5.7 | 0.8 | 0.8	|  46.0 | 6.0 |


Here is a link to my [code](https://github.com/tylerduke11/Semester-Project-386/blob/main/basketball.py) and my [data](https://github.com/tylerduke11/Semester-Project-386/blob/main/nba_data.csv) in my GitHub repository.

## Ethical Considerations
Web scraping has the potential for ethical concerns if the correct measures are not taken. I made sure to check the robots.txt pages on each website I scraped to ensure that I was scraping legal information from the websites. 


## Conclusion
I hope you enjoyed this project as much as I have as we explored the relationship between NBA player performance and salary.
