# EPL Home Advantage During COVID-19

Analysis of whether home advantage in the English Premier League
disappeared when matches were played without fans during the 2020-21
COVID-19 season.

## Question

Did home win rate actually drop during the fan-less 2020-21 season,
compared to normal seasons?

## Data

Match-level data for 11 EPL seasons (2014-15 through 2025-26, excluding
2019-20), including results, shots, fouls, cards, corners, and referee.

Source: [football-data.co.uk](http://www.football-data.co.uk/),
mirrored via [datahub.io](https://datahub.io/football/english-premier-league)

## Method

- Combined 11 seasons of match data and calculated home win rate per season
- Compared the COVID season (2020-21, no fans) against the 10 normal seasons
- Ran a two-proportion z-test to check whether the difference was
  statistically significant

Because the league, teams, and season structure stayed constant while
crowd presence was the main thing that changed, this comparison works
close to a natural experiment.

## Results

- COVID season home win rate: **37.9%** (144/380 games)
- Average across 10 normal seasons: **45.0%** (1,709/3,800 games)
- The COVID season was lower than every individual normal season in the
  comparison, including the weakest one (40.8%)
- Two-proportion z-test: **p = 0.0040** — the gap is unlikely to be due
  to random chance

## Limitations

- The 2020-21 season also involved a compressed fixture schedule and
  general pandemic disruption, which may have contributed to the drop
  alongside the absence of fans
- The 2019-20 season (which switched to no-fan matches mid-season) was
  excluded to keep the comparison clean
- The comparison window (2014-15 to 2024-25) was chosen for stylistic
  consistency; results might differ with earlier eras included
- Home advantage is influenced by many other factors (travel, rivalries,
  weather) not controlled for individually in this analysis

## Tools

Python, pandas, matplotlib, statsmodels, Google Colab
