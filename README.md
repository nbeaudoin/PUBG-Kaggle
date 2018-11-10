# PUBG-Kaggle
Kaggle competition submission for PUBG

Notebook for analysis in the 2018 Kaggle Competition for PUBG to predict probability of winning game based on 65,000 user profiles and over 18 million completed games.

(Below from Kaggle)

## Description

In a PUBG game, up to 100 players start in each match (matchId). Players can be on teams (groupId) which get ranked at the end of the game (winPlacePerc) based on how many other teams are still alive when they are eliminated. In game, players can pick up different munitions, revive downed-but-not-out (knocked) teammates, drive vehicles, swim, run, shoot, and experience all of the consequences -- such as falling too far or running themselves over and eliminating themselves.

You are provided with a large number of anonymized PUBG game stats, formatted so that each row contains one player's post-game stats. The data comes from matches of all types: solos, duos, squads, and custom; there is no guarantee of there being 100 players per match, nor at most 4 player per group.

**You must create a model which predicts players' finishing placement based on their final stats, on a scale from 1 (first place) to 0 (last place).**

## Evaluation Criteria

Submissions are evaluated on Mean Absolute Error between your predicted winPlacePerc and the observed winPlacePerc.

**Mean Absolute Error** (MAE) is the mean of the absolute value of the errors:

$$\frac 1n\sum_{i=1}^n|y_i-\hat{y}_i|$$

Submission File
For each Id in the test set, you must predict their placement as a percentage (0 for last, 1 for first place) for the winPlacePerc variable. The file should contain a header and have the following format:
