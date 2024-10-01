# Baseball Team Winning Rate Analysis

## Data source
University of Maryland Baseball Website (https://umterps.com/sports/basebal)

## Overview
* Employed Microsoft SQL Server to establish a database, integrating various data sources, performing data cleansing, and constructing specific queries to filter key data impacting the win rate
* Leveraged Tableau to develop intuitive visualizations and interactive dashboards, providing an in-depth analysis of the baseball team's performance to help improve the winning rate

## Project goal
This project aims to analyze and optimize the baseball team's winning rate by examining player distribution based on height and weight, and identifying performance trends influenced by temperature conditions

## Tools Used
* Microsoft SQL Server
* Tableau

## ER Diagram for Database Structure
![image/ER model.jpg](https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/ER%20model.jpg)

## Relational schema
Player(playerId, playerFirstName ,playerLastName, playerHeight, playerWeight)<br/>
Weather(weatherDate, weatherTemperature, gameld)<br/>
Schedule(gameId, gameOpponent ,gameStadium, gameDate)<br/>
Position(positionId, playerPosition)<br/>
Result(gameDate, winnerTeam , loserTeam, result)<br/>
Play(playerId, gameId)<br/>
Assign (playerId, positionId)

## Visualizaiton on Tableau

1.The chart was created to address how the coach distributes players based on their heights and weights. By showing the average height and weight for each position—pitching, fielding, and batting

<img width="80%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db%20Q1.jpg">


2.The chart shows that taller players are more common in pitching, particularly in winning games, while height seems to have less impact on batting and fielding outcomes. This may suggest height is more crucial for pitchers

![image/Q5.png](https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5.png)


