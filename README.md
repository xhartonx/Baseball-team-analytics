# University of Maryland Baseball Team Performance Analysis

## Data source
[University of Maryland Baseball Website](https://umterps.com/sports/baseball)

## Overview
This project employs **Microsoft SQL Server** and **Tableau** to analyze critical factors affecting the University of Maryland baseball team's win rate. The analysis focuses on player distribution (height and weight) and the influence of temperature conditions on performance.

- **Microsoft SQL Server**: Used for database management, integrating multiple data sources, data cleansing, and querying.
- **Tableau**: Used to create intuitive visualizations and interactive dashboards, providing insights to optimize the team’s win rate.

**Insights generated from the analysis can guide the coaching staff in optimizing player selection based on physical attributes and environmental factors, ultimately improving the team's performance.**

## Project goal
The primary goal of this project is to **optimize decision-making** by analyzing key performance indicators, such as player distribution and temperature trends, that contribute to game outcomes. The analysis specifically targets:
- Player distribution based on height and weight.
- Identifying performance trends influenced by temperature.

## Tools Used
- **Database Management**: Microsoft SQL Server
- **Visualization**: Tableau

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
Below are the insights derived from the visualizations built in Tableau.

### 1. Player Distribution Based on Height and Weight

- **Objective**: Analyze how the coaching staff distributes players by height and weight.
- **Key Insight**: The chart highlights the average height and weight for each position—pitching, fielding, and batting.

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db%20Q1.jpg">

### 2.1 Height's Impact on Winning
   
- **Objective**: Determine the role of player height in winning games.
- **Key Insight**: Taller players are predominantly chosen as pitchers, particularly in winning games. Height has less impact on batting and fielding success, suggesting its critical importance for pitching.

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5.png">

### 2.2 Weight's Impact on Winning
- **Objective**: Analyze the impact of player weight on game outcomes.
- **Key Insight**: Heavier pitchers tend to win more games compared to batters and fielders. Weight plays a significant role in pitching success, while batting and fielding positions show less variation in weight between winning and losing.

<img width="70%" alt="image" src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/Q5-2.png">

### 3. Temperature’s Impact on Performance
- **Objective**: Examine the correlation between temperature and team performance.
- **Key Insight**: Warmer temperatures, particularly during June, correlate with increased win rates, while colder weather in March leads to a dip in performance.

<img src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db03.jpg" alt="image" style="height:500px; width:auto;">

### 4. Win Rate Trends Across Seasons
- **Objective**: Identify win rate trends in different temperature conditions over several seasons.
- **Key Insight**: Colder temperatures tend to result in lower win rates across seasons, while warmer conditions correlate with better outcomes.

<img src="https://github.com/xhartonx/Baseball-team-analytics/blob/main/image/db04.jpg" alt="image" style="height:500px; width:auto;">

# Conclusion
By identifying critical factors such as height, weight, and temperature, this analysis provides actionable insights to guide the team's strategy. Adjustments in player selection and game scheduling could significantly enhance the team’s win rate, with warmer weather appearing to be a key factor for better performance.
