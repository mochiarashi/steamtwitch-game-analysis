# steamtwitch-game-analysis
Causal analysis of how Twitch viewership affects Steam gameplay using panel data and IV regression
# Steam & Twitch Game Analytics

## Project Overview
This project investigates the causal impact of Twitch viewership on Steam gameplay engagement using a large monthly panel of PC games.

The study links Twitch viewership, Steam player activity, and Google Trends search interest for 615 games from 2012 to 2024. The main goal is to determine whether Twitch exposure actively drives gameplay on Steam, rather than simply moving together with game popularity.

## Research Question
Does higher Twitch viewership causally increase Steam player engagement?

## Dataset
The project combines three data sources:

- Steam monthly player statistics
- Twitch monthly game viewership data
- Google Trends search interest data

The final panel covers 615 games across more than 100 monthly periods.

## Methodology
The analysis uses:

- Data cleaning and panel construction
- Log transformation of player and viewer variables
- Fixed effects regression
- Instrumental variables (IV / 2SLS)
- Lagged Google Trends as an instrument for Twitch viewership

Game fixed effects and month fixed effects are included to control for time-invariant game characteristics and common time shocks.

## Key Results
The fixed-effects OLS model shows a positive relationship between Twitch viewership and Steam players.

After correcting for simultaneity using IV-2SLS, the estimated causal effect becomes much larger: a 1% increase in Twitch viewership leads to approximately a 1% increase in Steam player engagement.

This suggests that Twitch is not only correlated with game popularity, but also acts as a powerful promotional channel that drives real gameplay behavior.

## Skills Demonstrated
- Python
- Pandas
- Data cleaning and merging
- Panel data analysis
- Fixed effects modeling
- Instrumental variables (IV / 2SLS)
- Causal inference
- Data visualization

## Files
- `steam_twitch_analysis.py`: main analysis script
- `README.md`: project summary

## Author
Chenhuan Ji  
Boston College  
MS in Applied Economics & Applied Analytics
