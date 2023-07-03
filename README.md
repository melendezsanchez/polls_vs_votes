# Presidential Elections in Latin America: Polls vs Votes since 2015

This repository contains the data used in our comparative analysis of Guatemala's June 25, 2023 presidential election.

The data and variables contained in each file are as follows:

### File 1: `candidate_data` (.xlsx, .csv)

Contains the following candidate-level data:

- `country`: County where election was held.
- `country_cd`: 2-3 character `country` abbreviation.
- `yr`: Year when the election was held.
- `had_runoff`: Takes a value of 1 if there was a runoff following this election, 0 otherwise.
- `candidates`: The total number of presidential candidates in the election.
- `name`: The candidate's first and last name.
- `last_name`: The candidate's last name.
- `polling_pct`: Expected vote share as per the poll(s) we examined.
- `voting_pct`: Realized vote share as per election returns.
- `polling_position`: Expected position as per the poll(s) we examined.
- `voting_position`: Realized position as per election returns.
- `vote_minus_poll`: Absolute measure electoral peformance vis-a-vis polls. Obtained by subtracting `polling_pct` from `voting_pct`.
- `vote_over_poll`: Proportional measure electoral peformance vis-a-vis polls. Obtained by dividing `voting_pct` by `polling_pct`.
- `position_change`: Another measure of electoral performance vis-a-vis polls. Obtained by subtracting `voting_position` from `polling_position`.
- `poll_name`: Name(s) of the poll(s) we examined.
- `exclusion`: If an election was excluded from our analysis, this variable provides a brief explanation. Otherwise, this variable is blank.

The file contains data for almost all elections and all candidates in Latin America between January 2015 and July 2023. As explained in our analysis, our calculations exclude data from candidates who received under 5% of the vote and from five elections (Bolivia 2019, Honduras 2017, Nicaragua 2016, Nicaragua 2021, and Venezuela 2018). However, data for these candidates and elections *are* included in this file (if available).

### File 2: `null_blank_votes` (.xlsx, .csv)

Contains the following data for each election:

- `country`: County where election was held.
- `yr`: Year when the election was held.
- `null_blank`: Null and blank votes as a percentage of total votes.
- `exclusion`: If an election was excluded from our analysis, this variable provides a brief explanation. Otherwise, this variable is blank.

The file contains data for almost all elections in Latin America between January 2015 and July 2023. As explained in our analysis, our calculations exclude data from five elections (Bolivia 2019, Honduras 2017, Nicaragua 2016, Nicaragua 2021, and Venezuela 2018). However, data for these  elections *are* included in this file (if available).

