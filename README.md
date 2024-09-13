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
* What are the average weight and height of the baseball team players in each position?
  
![image/db%20Q1.jpg](https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db%20Q1.jpg)
