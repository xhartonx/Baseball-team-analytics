# Baseball Team Winning Rate Analysis

## Data source
University of Maryland Baseball Website (https://umterps.com/sports/basebal)

## Overview
* Employed Microsoft SQL Server to establish a database, integrating various data sources, performing data cleansing, and constructing specific queries to filter key data impacting the win rate
* Leveraged Tableau to develop intuitive visualizations and interactive dashboards, providing an in-depth analysis of the baseball team's performance to help improve the winning rate

## Project goal
The goal of this project is to analyze and optimize the baseball team’s win rate. Specifically, the analysis focuses on:
- Player distribution based on height and weight.
- Identifying performance trends influenced by temperature conditions.

## Tools Used
- **Microsoft SQL Server**: For database management and querying.
- **Tableau**: For visualization and dashboard creation.

## ER Diagram for Database Structure

<img src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/ER%20model.jpg" alt="image" style="height:auto; width:70%;">

## Relational schema
The project’s relational schema defines the following entities and their relationships:
- **Player**: (playerId, playerFirstName, playerLastName, playerHeight, playerWeight)
- **Weather**: (weatherDate, weatherTemperature, gameId)
- **Schedule**: (gameId, gameOpponent, gameStadium, gameDate)
- **Position**: (positionId, playerPosition)
- **Result**: (gameDate, winnerTeam, loserTeam, result)
- **Play**: (playerId, gameId)
- **Assign**: (playerId, positionId)

## Visualizaiton on Tableau

### 1. Player Distribution Based on Height and Weight

The chart visualizes how the coaching staff distributes players by their heights and weights. It highlights the average height and weight for each position—pitching, fielding, and batting

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db%20Q1.jpg">


### 2.1 Player Height and Winning Impact
   
This chart reveals that taller players are predominantly chosen as pitchers, especially in winning games. However, height appears to have less impact on batting and fielding success. The data suggests that height is more critical for pitchers

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5.png">

### 2.2 Player Weight and Winning Impact

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5-2.png">

### 3. Impact of Temperature on Team Performance and Win Rate Trends

As temperatures rise throughout the season, the team’s win rate increases, peaking in June. Colder weather in March correlates with a slight dip in performance, suggesting warmer conditions may contribute to better results

<img src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db03.jpg" alt="image" style="height:500px; width:auto;">
