---
layout: post
title:  "Is NBA Player Performance Correlated with Player Salary?"
author: Tyler Duke
description: "An analysis of NBA players and their performance related to their salary"
date: Nov 30, 2023
image: "/assets/images/nba-banner.png"
--- 

## Introduction and Motivation
Have you ever wondered how NBA player performance is linked to their salary? Players make a lot of money but do the best players always get paid the most? I have always had this question in my mind because the best players should be getting paid the most. So, I decided to conduct an in-depth analysis of the data from the 2022-2023 NBA basketball season to determine if player performance is correlated with player salary. 

If you want to see a more detailed explanation of the project, such as how I quantify the "best" players, see [this](2023-11-14-semester-project.md) blog post I made at the beginning of my project.

In this blog post, I will display some of my findings as I explored the data through EDA (Exploratory Data Analysis). Here are some of my findings after exploring the data through EDA:

I first explored the trend between the average points of every player on a team compared to the average salary of every player on the team. I explored this with a side-by-side bar plot as shown below. A few interesting trends to note:
* The team with the highest average salary (by far) is the Los Angeles Clippers. This is justified, though, because they also have one of the highest average points.
* The San Antonio Spurs and the Houston Rockets seem to be getting the most bang for their buck. In other words, they are not playing their players as much compared to the points those players are getting them. This makes sense because those were among the worst teams in the NBA during the 2022-2023 season.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/bar_pts_vs_salary.png"/>

Here is another interesting graph. I have the average salary of each player on a team in the NBA compared to the other teams. We can see that the Toronto Raptors, for example, paid their players about $11 million on average.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/bar_salary_by_team.png"/>

I also looked at the distribution of points of each player on a team. So this graph can be interpreted that the Philidelphia 76ers had all the players on their team score an average of about 9 points throughout the season, with one player being an outlier scoring about 33 points on average. As we look at the data, this was likely Joel Embiid, as he was one of the highest-scoring players in the NBA during the 2022-2023 season.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/boxplot_team_points.png"/>

Here is a graph that shows a team's total wins vs the average salary of their players. The most interesting trend that we discover from this is that there is a positive trend in the data, indicated by the blue line. Thus, as a team spends more money on their players, they will win more games.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/point_teamwins_vs_salary.png"/>

This graph can be a little hard to interpret, but there are some interesting trends that come from this. I specifically look at the average points per game of each player vs their average salary. I specifically only look at the 3 teams with the highest average points (PHI, PHX, and NOP) and the 3 teams with the lowest average points (UTA, SAC, and CHI). We can see that there are a few players in the Phoenix Suns that have high salaries and high average points per game. So it seems that they are getting good value for those players also. Additionally, the Utah Jazz seem to have a few players who are scoring a lot of points per game but are not paid as much as other players.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/top3_bottom3_score.png"/>

This is a large graph that can show a lot of interesting trends. I explored the relationship between 10 different player metrics across the entire NBA and their average salary. Metrics include: Age, Games Played, Field Goal %, 3 Point %, Free Throw %, Points, Rebounds, Assists, Double Doubles, and Triple Doubles. We see a positive relationship in each of the metrics, which is to be expected. The most interesting trends that I found were that for the Field Goal % and 3 Point %, both have only slightly positive trends. This means that the players who get paid the most still get about the same percentage of made baskets as the players who are paid the least.
<img src="{{site.url}}/{{site.baseurl}}/assets/images/multi_salary_vs_metrics.png"/>


Let me know if there are other interesting things I can explore with this data! These were just a few of my findings from my exploratory data analysis.


Here is a link to my [code](https://github.com/tylerduke11/Semester-Project-386/blob/main/eda.py) I used for EDAand my [data](https://github.com/tylerduke11/Semester-Project-386/blob/main/nba_data.csv) in my GitHub repository.
