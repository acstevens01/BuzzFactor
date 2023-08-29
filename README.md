# BuzzFactor
This repository contains all the code for the thesis: Buzz factor bias: Using the wisdom of crowds to try beat the bookies

The code is ordered as presented in the paper.
## Replication
This code replicates the original paper: [Betting on a buzz: Mispricing and inefficiency in online sportsbook](https://www.sciencedirect.com/science/article/pii/S0169207022001091)
### Ramirez Data
This contains the code to pre-process the original dataset, apply a replicated method and then correct the issues associated.
- stats_their_data.ipynb: generates the statistics need to replicated Ramirez using their data.
- final_their_data.ipynb: uses Ramirez data with our replicated methodology to validate results.
- corrections_their_data.ipynb: applies corrections to their methododlogy and applies it to their data.
### Stevens Data
This contains the code to generate an expanded dataset, then applies the corrected methododlogy to an unclean and clean version of the data.
- complie_results_1.ipynb: gathers the WTA results for the extended time period and saves a cleaned and uncleaned version.
- players_2.ipynb: generates the Wikipedia page titles for each player in the dataset.
- wikipedia_3.ipynb: generates the daily Wikipedia page view data for each player.

There are two folders Uncleaned and Cleaned which have almost identical code but one deals with the uncleaned dataset and each file therefore has the ending '_unclean.ipynb'.
- merge_4.ipynb: merges the odds/results dataset with the generated Wikipedia data.
- stats_5.ipynb: generates the necessary statistics for each match and removes null values.
- final_6.ipynb: applies the corrected methodology and trains and tests the model to generate results.
## Extension
This code extends the corrected methodology to apply it to 3 new sports.
### Football
This code generates a football dataset with results, odds and Wikipedia data for the top 5 European league 2015-2023 and applies the corrected methodology. 
- football_complie_results_1.ipynb: gathers the results for all 5 leagues.
- football_teams_2.ipynb: generates the Wikipedia page titles for each team in the dataset.
- football_wikipedia_3.ipynb: generates the daily Wikipedia page view data for each team.
- football_merge_4.ipynb: merges the odds/results dataset with the generated Wikipedia data.
- football_stats_5.ipynb: generates the necessary statistics for each match and removes null values.
- football_final_6.ipynb: applies the corrected methodology and trains and tests the model to generate results.
### Men's tennis
This contains the code to generate a men's tennis dataset with all ATP matches, then applies the corrected methododlogy to an unclean and clean version of the data.
- mens_tennis_complie_results_1.ipynb: gathers the ATP results from 2015-2023 and saves a cleaned and uncleaned version.
- mens_tennis_players_2.ipynb: generates the Wikipedia page titles for each player in the dataset.
- mens_tennis_wikipedia_3.ipynb: generates the daily Wikipedia page view data for each player.

There are two folders Uncleaned and Cleaned which have almost identical code but one deals with the uncleaned dataset and each file therefore has the ending '_unclean.ipynb'.
- mens_tennis_merge_4.ipynb: merges the odds/results dataset with the generated Wikipedia data.
- mens_tennis_stats_5.ipynb: generates the necessary statistics for each match and removes null values.
- mens_tennis_final_6.ipynb: applies the corrected methodology and trains and tests the model to generate results.
### UFC
This code generates a UFC dataset with results, odds and Wikipedia data for all fights in 2015-2021 and applies the corrected methodology. 
- UFC_odds_1.ipynb: complies results and converts odds from American to decimal.
- UFC_players_2.ipynb: generates the Wikipedia page titles for each fighter in the dataset.
- UFC_wikipedia_3.ipynb: generates the daily Wikipedia page view data for each fighter.
- UFC_merge_4.ipynb: merges the odds/results dataset with the generated Wikipedia data.
- UFC_stats_5.ipynb: generates the necessary statistics for each fight and removes null values.
- UFC_final_6.ipynb: applies the corrected methodology and trains and tests the model to generate results.