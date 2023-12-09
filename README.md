
backfill - backfills data from now to the start of the season. Generates nba_games.csv. This is player/game level data

calculate_stats - calculates game level stats from nba_games.csv. Generates game_stats.csv.

train_model

predict_nba_game_outcomes - gets all nba games for the current day and predicts the outcome of each game. Generates or updates nba_game_predictions.csv

get_actual_nba_game_outcomes - gets all nba games for the current day and updates the actual outcome of each game. Updates nba_game_predictions.csv