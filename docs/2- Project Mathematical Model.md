# Teamfight Tactics Optimization Project

## Objective:

Apply linear and constrained optimization techniques to create a sophisticated model for the Teamfight Tactics (TFT) leveling guide, considering dynamic factors such as gold management, health preservation, champion pool percentages, stage/round details, gold interest, and win/loss streaks.

## Mathematical Model:

### Decision Variables:

- $Gold_{level\_up}$: Amount of gold allocated for leveling up.
- $Gold_{roll}$: Amount of gold allocated for rolling.
- $Gold_{interest}$: Gold interest earned based on savings.
- $Gold_{streak}$: Gold earned from win/loss streaks.
- $Gold_{saved}$: Total gold saved.

### Objective Function:

Maximize overall board strength considering champion star levels, synergy bonuses, and gold efficiency.

$$Board\_Strength = \sum_{i} (Star\_Level_i \times Synergy\_Bonus_i)$$

### Constraints:

1. **Gold Constraint:**
    $$Gold_{level\_up} + Gold_{roll} + Gold_{saved} + Gold_{streak} + Gold_{interest} \leq Total\_Gold_{available}$$

2. **Health Preservation Constraint:**
    $$Current\_Health \geq Minimum\_Health$$

3. **Champion Pool Constraint:**
    Ensure that champion pool percentages are satisfied.

4. **Stage and Round Constraint:**
    Consider dynamic constraints based on the current stage and round.

5. **Gold Interest Constraint:**
    $$Gold_{interest} = \lfloor Gold_{saved} \div 10 \rfloor$$

6. **Gold Streak Constraint:**
    Determine gold streak bonus based on win/loss streak.

7. **Champion Availability Constraint:**
    Adjust champion availability based on the current stage and round.

## Implementation:

Utilize Python programming to solve the linear programming problem and dynamically adjust constraints based on the evolving state of the game.
