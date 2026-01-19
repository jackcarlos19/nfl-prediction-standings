### ESPN NFL Playoff Prediction Pool — Matchup Alignment Snapshot (Corrected)

This update is based **only** on the verified bracket data in `super_bowl_brackets_normalized.json` (12 contestants total).  
It **removes** the previously ungrounded claims about betting-line simulations, “100,000 tournaments,” and any odds/points that can’t be computed without official game results + your pool’s scoring config.

#### Scoring rules (as provided)

- **Wild Card**: 1 point per correct winner (matchups are fixed, so “correct matchup” is automatic)
- **Divisional**: 2 points per game, **only if** the predicted matchup occurred **and** the predicted winner is correct
- **Conference Championship**: 3 points, **only if** the predicted matchup occurred **and** the predicted winner is correct
- **Super Bowl**: 4 points, **only if** both teams are correct **and** the winner is correct

#### Correct-matchup focus (Divisional Round)

Using the divisional matchups you referenced:
- **NFC**: SEA–SF, CHI–LAR  
- **AFC**: DEN–BUF, NE–HOU  

Here’s who has those **exact matchups** present in their divisional round:

| Contestant | SEA–SF | CHI–LAR | DEN–BUF | NE–HOU | Total Hits (0–4) |
|-----------|:------:|:-------:|:-------:|:------:|:---------------:|
| Bere |  |  | ✓ | ✓ | 2 |
| Carlos |  |  | ✓ | ✓ | 2 |
| Chavito |  |  | ✓ | ✓ | 2 |
| Mario | ✓ | ✓ |  |  | 2 |
| Ruben | ✓ | ✓ |  |  | 2 |
| David G. |  |  | ✓ |  | 1 |
| Jayden | ✓ |  |  |  | 1 |
| Beto |  |  |  |  | 0 |
| chucky |  |  |  |  | 0 |
| Chuy |  |  |  |  | 0 |
| David L. |  |  |  |  | 0 |
| Liz |  |  |  |  | 0 |

**Key correction vs the prior write-up:** nobody has a “perfect alignment so far” on all four divisional matchups (no one is 4/4) based on the brackets in the JSON.

#### Why the original “Points / Max Possible / Odds” table can’t be corrected from the JSON alone

Now that we have the scoring rules, the remaining missing ingredient is **actual results** (winners + which matchups occurred).

To produce a real, deterministic leaderboard (**Points** and **Max Possible**), please provide the outcomes that are “locked” so far:
- Wild Card winners (all 6 games)
- Any completed Divisional games (matchup + winner)

Then I can compute standings deterministically from `super_bowl_brackets_normalized.json` (no simulations, no betting lines).

