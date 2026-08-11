# EPL Home Advantage During COVID-19

Home advantage in the English Premier League dropped when matches were played without fans during the 2020-21 COVID-19 season, suggesting crowds genuinely influence match outcomes, not just atmosphere.

## Results

Home win rate during the COVID season came out to 37.9% (144 out of 380 games), compared to an average of 45.0% (1,709 out of 3,800 games) across 10 normal seasons. It was lower than every single normal season in the comparison, including the weakest one at 40.8%. A two-proportion z-test put the p-value at 0.0040, meaning this gap is unlikely to be random chance.

## Method

I combined 11 EPL seasons (2014-15 through 2025-26, excluding 2019-20), calculated home win rate for each one, then compared the fan-less 2020-21 season against the 10 normal seasons using a two-proportion z-test. Since the league, teams, and season length stayed the same and crowd presence was really the only thing that changed, this works out close to a natural experiment.

## Data

Match-level data for 11 EPL seasons, covering results, shots, fouls, cards, corners, and referees.

Source: [football-data.co.uk](http://www.football-data.co.uk/), mirrored via [datahub.io](https://datahub.io/football/english-premier-league)

## Limitations

The 2020-21 season also had a compressed schedule and general pandemic disruption, so some of the drop could be fatigue-related rather than purely about fans. The 2019-20 season was excluded since it switched to no-fan matches partway through. The comparison window starting at 2014-15 was a somewhat arbitrary cutoff, chosen mainly to keep playing styles roughly consistent across seasons. Home advantage also depends on plenty of other things, like travel and rivalries, that this analysis doesn't account for individually.

## Tools

Python, pandas, matplotlib, statsmodels, Google Colab
