# NBA Model

Simple model for predicting the outcome of NBA games

### Notebooks

#### historical_data

Backfills historical (player/game level) data for a given nba season. Kept running into limitations of the API so there is a built in 10 second wait in there after each 100 requests to help it cool down. Doing more than one season at a time failed often so right now just does one season at a time.

#### backfill_season

Backfills data from now to the start of the season. Generates nba_games.csv. This is player/game level data

#### calculate_stats 
Fetches latest data and calculates game level stats from nba_games.csv. 10 day, 5 day averages are calculated, as well as season statistics and ELO. Generates game_stats.csv.

#### train_model

Pretty self explanatory 

#### predict_nba_game_outcomes 

Gets all nba games for the current day and predicts the outcome of each game. Generates or updates predictions.csv

#### get_actual_nba_game_outcomes 
TODO