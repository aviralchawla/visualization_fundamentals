# Data

The data in the repository is sourced from two Kaggle repositories. Here is a brief overview of the datasets-

## 1. Steam Charts

### Overview

This dataset contains information about the average & peak monthly number of players per 6725 unique games placed on Steam. Originated from <https://steamcharts.com>

### Source 

<https://www.kaggle.com/datasets/lunthu/steam-monthly-average-players>

### Files

`steamcharts.csv`

- `Month` - month-year of observation
- `avg_players` - average players count (float)
- `gain` - difference comparing to previous month (float)
- `gain_percent` - difference comparing to previous month in percents (float)
- `peak_players` - highest value of players at the same time for selected month (float)
- `name` - name of the game (string)
- `steam_appid` - steam ID of the game (string)

## 2. Diabetes Health Indicators

### Overview

The Behavioral Risk Factor Surveillance System (BRFSS) is an ongoing, state-based telephone survey that collects data about health-related risk behaviors, chronic health conditions, and the use of preventive services among adults aged 18 years and older residing in the United States. Conducted annually by the Centers for Disease Control and Prevention (CDC), the BRFSS has been providing valuable insights into the health status and behaviors of U.S. adults since its inception in 1984.

### Source 

<https://www.kaggle.com/datasets/julnazz/diabetes-health-indicators-dataset>

### Files

`diabetes/diabates_012.csv`
A clean dataset of 236,378 survey responses to the CDC's BRFSS2021. The target variable `Diabetes_012` has 3 classes. `0` is for no diabetes or only during pregnancy, `1` is for prediabetes, and `2` is for diabetes. There is class imbalance in this dataset. This dataset has 21 feature variables.


`diabetes/diabetes_01_balanced.csv`
A clean dataset of 67,136 survey responses to the CDC's BRFSS2021. It has an equal 50-50 split of respondents with no diabetes and with either prediabetes or diabetes. The target variable `Diabetes_binary` has 2 classes. `0` is for no diabetes, and `1` is for prediabetes or diabetes. This dataset has 21 feature variables and is balanced.

`diabetes/diabetes_01.csv`
A clean dataset of 236,378 survey responses to the CDC's BRFSS2021. The target variable `Diabetes_binary` has 2 classes. `0` is for no diabetes, and `1` is for prediabetes or diabetes. This dataset has 21 feature variables and is not balanced.
