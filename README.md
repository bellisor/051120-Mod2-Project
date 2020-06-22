# Flatiron Data Science Project 2: Linear Regression

## Primary Goals:

## Introduction
The National Hockey League (NHL) is one of the largest organization for professional hockey. Players from all over the world participate in 31 franchises across North America. 

### Business Case
As a coach looking at goal scoring, do aggressive play styles lead to more goals? 

### About our Data
Our data set was downloaded from https://www.kaggle.com/martinellis/nhl-game-data?select=game_plays.csv

There are several different .csv files from the source, the ones relevent to this project are:
* game_skater_stats.csv
* game_plays.csv
* player_info.csv
* game_teams_stats.csv
* team_info.csv

From these datasets, we merged them into one dataframe. The dataframe still contained observations for every game. 

The next step was to summarize on a season level, so the dataframe was aggregated to contain season observations for each player.

The data is also focused on the 5 skaters (no goalie data) with an emphasis on even ice time (5v5). 

Two Features were created to add into the model:
* TakeawayDiff - take away diffrential which is the difference between the amount of takaways a player had in season and the amount of giveaways a player had

* faceOffWinP - Face off win percentage which is the amount of a face offs a player won divided by the 



## Methodology
1. Data Collection

2. Data Wrangling

3. EDA and Visualization

4. Hypothesis Testing

5. Model Development

6. Cross Validation

## Results
Upon review of the data, there is a statistical relationship between aggressive play and goal scoring. That relationship however is that players with less hits score more goals than players with a high amount of hits. This can be explained by players with a high amount of hits also have a high amount of penalty minutes and therefore less amount of time on the ice. 

When evaluating the importance of features the three features with the highest coefficients were:

* Number of shots
* Amount of time on ice
* Number of hits

Model R^2 is 0.85

The model has a high r^2 and an accuracy score of 98%

Train Mean Squarred Error: 14.720119406131744
Test Mean Squarred Error: 13.939463556526688

The Mean Squarred Error of the training data is very close to the MSE of the Test Data, which is very good. 

An intersting note is that the MSE of the Test data is lower than the MSE of the training data which is rare.




## Conclusion
The goal of this project was to see how aggresive playing styles have an impact on scoring chances. According to the model, players with an average amount of hits have a higher amount of goals scored. Howevr, players with a higher amount of penalty minutes have less goals. This makes sense because being in the penalty box takes away from a players time on ice and therefore limits the amount of shots a player can take. The amount of shots a player takes is the most correlated factor to amount of goals scored. Therefore, when you're watching your next hockey game and crowd yells "SHOOT!" there is some significance to it. 

- "You miss 100 percent of the shots you never take" - Wayne Gretzky, 'The Great One'



## Interesting Insights

The average hockey player spends 16.55 minutes on the ice in a given game. 

Players position on the ice has a statistical relationship with their nationality

Centers have the most amount of points (goals+assists) in a season.

Canadiens have the most amount of points but also the highest population in the NHL.




