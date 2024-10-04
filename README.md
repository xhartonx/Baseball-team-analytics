# Baseball Team Winning Rate Analysis

## Data source
University of Maryland Baseball Website (https://umterps.com/sports/basebal)

## Overview
* Employed Microsoft SQL Server to establish a database, integrating various data sources, performing data cleansing, and constructing specific queries to filter key data impacting the win rate
* Leveraged Tableau to develop intuitive visualizations and interactive dashboards, providing an in-depth analysis of the baseball team's performance to help improve the winning rate

## Project goal
The goal of this project is to analyze and optimize the baseball team’s win rate. Specifically, the analysis focuses on:
* Player distribution based on height and weight.
* Identifying performance trends influenced by temperature conditions.

## Tools Used
* Microsoft SQL Server: For database management and querying.
* Tableau: For visualization and dashboard creation.

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

### 1. Player Distribution Based on Height and Weight

The first chart visualizes how the coaching staff distributes players by their heights and weights. It highlights the average height and weight for each position—pitching, fielding, and batting

<img width="80%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db%20Q1.jpg">


### 2. Player Height and Winning Impact
   
This chart reveals that taller players are predominantly chosen as pitchers, especially in winning games. However, height appears to have less impact on batting and fielding success. The data suggests that height is more critical for pitchers

<img width="80%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5.png">


### 3.

<img height="50%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db03.jpg">
