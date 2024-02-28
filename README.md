
# Remix Rumble NA Regionals Data 

## TFT Background Info
- https://www.thegamer.com/teamfight-tactics-complete-beginners-guide-tips/
- Relevant sections to this analysis:
  - What is the Carousel?
  - How do Items work?
  - What are PvE Rounds?

## Project Goals
In this analysis we will perform a variety of data science tasks:
- Exploratory Data Analysis to identify possible patterns, anomalies, relationships within the data as well as develop hypotheses for deeper analysis
- Predictive modeling to determine how strongly early game decisions and randomness affect player placement and whether we can leverage this knowledge to build a model with meaningful predictive power
- Diagnostic Analysis in looking deeper in the data and TFT core game mechanics to make informed decisions regarding feature selection
- Model Insights to, through the lens of our analysis, discuss whether core TFT game mechanics are well designed and whether or not certain aspects need rebalancing

## Data Overview
- Data is gathered manually from Twitch Videos on Demand (VODs) from each player in the Remix Rumble NA Regional Tournament for Day 2 and Day 3. Tourney data is not captured entirely in this dataset as some players failed to save their VODs from either or both days.

## Column Descriptors
- neeko: number of neeko (champion duplicator) on Stage 1 (no duplicator -> 0, lesser duplicator -> 1, greater duplicator -> 2)
- gold_not_units: receiving a gold drop rather than a unit drop on Stage 1, binary
- 3cost: number of 3-costs obtained on Stage 1
- open_{item}: opening with {item} on Stage 1, binary
- pick_order: champion pick order on 2-4 carousel (1st -> 1, 2nd -> 2, 3rd -> 3, 4th -> 4)
- prekrug_slams: number of completed items by krugs (2-7). Items completed after 2-6 combat and on 2-7 do not count.
- points: points gained during game
- placement: placement of game (9-points)
