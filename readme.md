Try to build a goated FPL roster

find what numbers are truly correlated - what things are truly coordinated by using mathematics. but first, the data, backtest on previous years. try to think if more data is needed or not.

Plan/Brainstorming:

Get the 25 registered player roster. For every single registered player, get their stats for every player. try to make a data driven decision on my final fpl roster & try to win a league or two.

For new/transfer players for this season maybe try to get the stats from their previous years? <- this will be hard to to do but I think first should focus on premier league only statistics and then later maybe add stats from other leagues and such

Only get 25 players, and only allow for 25 players to registered

So have a constraint that a team_id can only have 25 player_id where registered == true

Fantasty premier league started in 2002 so i have that much data for any currently active players.

datasources - sofascore, footballref, transfermrkt

Tables in my DB:

## Players

---

player_id player_name nationality_id

## Teams

---

team_id team_name league_id

## Positions

---

position_id position_abbr position_name

## General_Stats

---

player_id match_id goals_scored assists passes_completed passes_attempted tackles_won tackles_attempted interceptions fouled_against fouls_committed yellow_cards red_cards handeballs penalty_conceded penalty_won turnover progressive_carry dribbles_completed dribbles_attempted minutes_played aerial_rate penalties_scored

shots shots_on_target shots_off_target shots_blocked key_passes shot_creating_actions touches_in_opposition_box offsides touches_final_third

progressive_passes passes_into_final_third crosses_completed crosses_attempted through_balls touches_midfield

clearances match_id blocked_shots blocked_passes blocked_crosses pressure_successful pressure_total ground_duel_won ground_duel_total aerial_duel_won aerial_duel_total ball_recoveries defensive_actions_x_90 touches_defensive

saves_in_box saves_outside_box saves_total save_percentage clean_sheets goals_conceded post_shot_xg_faced crosses_blocked sweeper_actions

pl_base_points fpl_bonues_points current_price

## Match_Results

---

match_id home_team_id away_team_id home_score away_score referee_id season_id

## Referee

---

referee_id referee_name

## Nationality

---

nationality_id nationality_name

## League

---

league_id league_name

## Season

---

season_id season_name

## Rosters

---

roster_id player_id team_id season_id position_id season_start_price
