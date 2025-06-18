# nba_raptor 

A lightweight Python project to explore and analyze RAPTOR metrics in the NBA, based on two CSV datasets:
- `modern_RAPTOR_by_player.csv` – holds RAPTOR ratings for individual players.
- `modern_RAPTOR_by_team.csv` – contains aggregated RAPTOR ratings at the team level.



## 📁 Data Files

| File                                       | Description                                        |
|--------------------------------------------|----------------------------------------------------|
| `modern_RAPTOR_by_player.csv`             | Player-level RAPTOR ratings                        |
| `modern_RAPTOR_by_team.csv`               | Aggregated team-level RAPTOR metrics               |

---

## Poject Structure

### `modern_RAPTOR_by_player.csv`

| Column           | Description                                                                 |
|------------------|------------------------------------------------------------------------------|
| `player_id`      | Unique identifier for each player                                           |
| `player_name`    | Full name of the player                                                     |
| `season`         | NBA season (e.g., `2023-24`)                                                |
| `minutes_played` | Total minutes played during the season                                      |
| `offensive_RAPTOR` | Measure of player’s impact on offense (per 100 possessions)               |
| `defensive_RAPTOR` | Measure of player’s impact on defense (per 100 possessions)               |
| `total_RAPTOR`    | Combined overall RAPTOR rating (offensive + defensive)                     |
| *[additional columns]* | Any extra stats like pace-adjusted metrics, per-36 numbers, etc.      |

---

### `modern_RAPTOR_by_team.csv`

| Column            | Description                                                               |
|-------------------|---------------------------------------------------------------------------|
| `team_id`         | Unique team identifier (e.g., `LAL`, `BOS`)                              |
| `team_name`       | Full team name (e.g., “Los Angeles Lakers”)                              |
| `season`          | NBA season (e.g., `2023-24`)                                              |
| `offensive_RAPTOR` | Team’s per-100-pos offensive RAPTOR                                    |
| `defensive_RAPTOR` | Team’s per-100-pos defensive RAPTOR                                    |
| `total_RAPTOR`     | Combined team RAPTOR score                                              |
| `wins`             | Number of wins in the season                                            |
| `pace`             | Team possession pace (possessions per 48 minutes)                       |
| *[additional columns]* | Other aggregated metrics like net rating, eFG%, etc.              |

---

## 🚀 Getting Started

### Requirements

- Python 3.x  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

```bash
pip install pandas numpy matplotlib 
