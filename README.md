# Soccer-Match-Winner-Predictions---EPL

The project aim to utilise historical data for the English Premier League matches found on the API located at https://api.football-data.org/ to predict outcomes of future soccer matches.
The final model has to be able to predcit three classes i.e. draw(0), home win(1) or away win(2)

Python programming language and its libraries are utilized to achieve this. Due to the degree of cleanliness the data is, a lot of energy was directed into feature engineering and machine learning modelling rather than on cleaning of the data.

The data retrieved:
  - Previous season's matches data
  - Previous season's final log standings.
  - Current season's matches data

The season's matches data includes:
  - date (including the team) the matche was played or is scheduled for
  - home team
  - away team
  - the score, if the game has been played
  - the name of the referee
  - the winner of the game
  - the match day

From the above mentioned data, additional features are engineered to improve on the modelling. Some of which are mentioned below:
  - the home and away team's winning streaks before playing the current match
  - the home's and away team's average goals per match before playing the current match
  - whether the day the match is played is a weekend or not
  - the head-to-head results of the two teams playing together
  - the current log position of both the home and away team.

# Machine Learning Modelling

Three different models were trained once the data had been prepared to compare which had better performance.
The trained models are:
  - RandomForest
  - LogisticRegression
  - DecisionTree

To evaluate this, sklearn's libraries for accuracy, precision, recall and F1 score was utilized. Additionally the confusion matrices were utilized.
Of the three models, DecisionTrees showed to be favourable due to its abilities to correctly identify best the three classes than the other two models.


# Libraries

sklearn
pandas
requests
os
matplotlib
seaborn

