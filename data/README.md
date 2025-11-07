# Data

The data in the repository is sourced from two Kaggle repositories. Here is a brief overview of the datasets-

## Steam Charts

### Overview

This dataset contains information about the average & peak monthly number of players per 6725 unique games placed on Steam. Originated from <https://steamcharts.com>

### Source 

<https://www.kaggle.com/datasets/lunthu/steam-monthly-average-players?resource=download>

### Files

`steamcharts.csv`

- `Month` - month-year of observation
- `avg_players` - average players count (float)
- `gain` - difference comparing to previous month (float)
- `gain_percent` - difference comparing to previous month in percents (float)
- `peak_players` - highest value of players at the same time for selected month (float)
- `name` - name of the game (string)
- `steam_appid` - steam ID of the game (string)

