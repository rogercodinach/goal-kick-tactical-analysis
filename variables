# Variables Description – Bayer Leverkusen Goal Kick Dataset

This document describes the main variables used in the tactical analysis of goal kicks. Variables are grouped by category: match info, player info, event info, spatial context, and tactical scoring.

---

## 1. Match Information
| Variable | Description |
|----------|-------------|
| `match_id` | Unique identifier for each match |
| `match_date` | Date of the match (YYYY-MM-DD) |
| `competition` | Name of the competition (e.g., GER.1) |
| `competition_stage` | Stage of the competition (e.g., Regular Season, Playoffs) |
| `match_week` | Week number of the match in the season |
| `competition_phase` | Competition phase code |
| `season` | Season year (e.g., 2023/2024) |
| `home_team` | Name of home team |
| `away_team` | Name of away team |
| `local_team` | Boolean indicating if Bayer Leverkusen is the home team |
| `stadium` | Name of the stadium |
| `home_score` / `away_score` | Final match score for home and away teams |

---

## 2. Event Information
| Variable | Description |
|----------|-------------|
| `id` | Unique identifier for each event in the match |
| `period` | Match period (e.g., 1st half, 2nd half) |
| `match_moment` | Time elapsed in the period (minutes:seconds) |
| `timestamp` | Precise timestamp of the event (HH:MM:SS.milliseconds) |
| `irt_result` | Score at the time of the event (team vs rival) |
| `irt_team_score` / `irt_rival_score` | Goals scored by team and opponent at event time |
| `irt_goal_difference` | Difference in goals at event moment |

---

## 3. Player & Team Information
| Variable | Description |
|----------|-------------|
| `team` | Team performing the goal kick |
| `player` | Player executing the goal kick |
| `position` | Player position at the time of the event |
| `start_location` | `[x, y]` coordinates of the player at event start |
| `pass_recipient` / `pass_recipient_id` | Player receiving the pass, if any |
| `pass_recipient_position` | Position of pass recipient |

---

## 4. Pass / Goal Kick Attributes
| Variable | Description |
|----------|-------------|
| `type` | Event type (Pass / Goal Kick) |
| `pass_type` | Specific type of pass (Goal Kick, Short Pass, etc.) |
| `pass_body_part` | Foot used to perform the pass |
| `pass_end_location` | `[x, y]` coordinates where the ball ends |
| `pass_length` | Distance of the pass (meters) |
| `pass_height` | Height type (Ground, Low, High) |
| `pass_outcome` | Pass outcome (Complete / Incomplete) |
| `duration` | Duration of the event in seconds |

---

## 5. Spatial Context – Teammates & Opponents
| Variable | Description |
|----------|-------------|
| `teammate_1` … `teammate_10` | IDs or positions of closest teammates at event moment |
| `rival_1` … `rival_11` | IDs or positions of closest opponents |
| `teammate_distance_1` … `teammate_distance_10` | Distance (meters) to each nearby teammate |
| `rival_distance_1` … `rival_distance_11` | Distance (meters) to each nearby rival |
| `close_teammates` | Count of teammates within a 10m radius |
| `passing_ratio_team` | Team’s pass frequency ratio at event moment |
| `passing_ratio_label_team` | Categorized game tempo label (e.g., Low, Medium, High) |
| `passing_ratio_match` | Overall pass ratio in match |
| `passing_ratio_label_match` | Categorized match-level tempo |
| `passes_before_event` | Number of passes executed by team before the goal kick |

---

## 6. Tactical Context
| Variable | Description |
|----------|-------------|
| `matchscore_pressure` | Score pressure at event time (leading, drawing, trailing) |
| `freespace_score` | Score representing available space for execution |
| `prev_GK` | Previous goalkeeper event ID |
| `prev_Gk_score_std` / `prev_Gk_score_mean` | Std and mean of previous goal kick tactical scores |

---

## 7. Tactical Evaluation
| Variable | Description |
|----------|-------------|
| `score_level` | Categorical tactical score (e.g., Low, Medium, High) |
| `score` | Numeric score computed by rule-based model, evaluating tactical execution quality |

---

> All variables are aligned with the methodology applied in the project, allowing quantitative and contextualized analysis of tactical patterns in goal kick situations.
