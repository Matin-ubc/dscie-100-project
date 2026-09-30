# Women's NCAA March Madness — Final Four Prediction

This project analyzes Women's NCAA March Madness data from 1982–2018 to investigate:

Can a team's conference wins and regional wins be used to predict whether the team reaches the Final Four?

## Method

A k-nearest neighbors (k-NN) classification model was used to predict whether a team reached the Final Four.

- Predictors: conf_wins, reg_wins
- Response: made_top4 (Yes/No)
- 75% training / 25% testing split
- 10-fold cross-validation
- Missing values handled using mean imputation
- Best value of k: 9

## Results

The final model achieved a 71.4% precision when predicting teams that reached the Final Four.

The analysis suggests that conference and regional wins provide useful information for predicting Final Four appearances, although they do not perfectly predict the outcome.

## Tools
- R
- tidyverse
- tidymodels
- ggplot2

### Generative AI Disclosure

Generative AI was used to help debug an error caused by missing values during model training. It helped identify step_impute_mean() as an appropriate way to handle the missing values.
