# FPL model plan
Tom Conway

## Plan - what do I need to do and status of each

## Start as a GitHub project?

- Explore GitHub and make it work - Done

## Overarching structure

- work out headline model and create different files which will hold the
  engines. Rest of tasks are based on what was used last time.
  - Format of different files - I think make each an R file, which runs
    a specific engine. Then the engines each modify data tables that are
    carried across between.
  - For each engine we have a QMD file which has a description of how it
    works? No - that has to contain the model, we don’t want it in two
    separate places. Instead we break down the functions into different
    files - and render them in order?
  - This is an experiment - R code feels more natural, but QMD will help
    communicate it.
- So - I will create each of the below files as QMDs.

## Get data

- Scrape from FPL API

- Find data of results by team

- Other team or player data?

- Get Opta projections

## Predict the scores of matches based on the teams involved

- Import historic team score data

- Create a model for projecting the scores of future fixtures - poisson
  attack vs defence scores + home advantage + exponential time weighting
  backoff

## Predict player scores

- Import player data

- Model different kinds of player scores:

  - Goalkeeper

  - Defender

  - Midfielder

  - Striker

- Prediction for each player score for future games

## Pick a team

- Create and model algorithm for picking players to make up a 15

## Add other features of the game

- Injuries

- Transfers

- Chips

- Newly promoted teams

- New players

- Bonus points

- Yellow cards

## Refining and modelling

- Create season emulator for projecting the performance of different
  models across the season / for predicting the next gameweek

- Think of different options for model - both in individual elements and
  in overarching structure

- Try out different algorithms for each part of the model and evaluate
  them
