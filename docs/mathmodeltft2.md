# Application of Linear and Constrained Optimization in TFT Leveling Guide

## Objective Function (Linear Programming):
Maximize Board Strength: Formulate an objective function that maximizes the overall strength of your board. This includes considering the star level of champions, synergy bonuses, and gold efficiency.

## Decision Variables (Linear Programming):
Gold Allocation: Define decision variables for the amount of gold to be allocated between leveling up and rolling for champions.

## Constraints (Constrained Optimization):
**Gold Constraint:**
Limit the total gold expenditure based on the available gold. This ensures that the strategy is feasible within the current financial constraints.

**Health Preservation Constraint:**
Set a constraint to maintain a minimum level of health. This ensures that the optimization accounts for health preservation while making leveling and rolling decisions.

**Champion Pool Constraint:**
Ensure that the optimization considers the available champion pool percentages at each level. This prevents overcommitting to specific units and maintains a balanced champion pool.

## Formulation Example:
**Maximize:**
\[ \text{Board Strength} = \sum_{i} (\text{Star Level}_i \times \text{Synergy Bonus}_i) \]

**Decision Variables:**
\[ \text{Gold}_{\text{level up}}, \text{Gold}_{\text{roll}} \]

**Constraints:**
\[ \text{Total Gold} = \text{Gold}_{\text{level up}} + \text{Gold}_{\text{roll}} \leq \text{Available Gold} \]
\[ \text{Health} \geq \text{Minimum Health} \]
\[ \text{Champion Pool Percentages are satisfied.} \]

By combining Linear Programming and Constrained Optimization, you create a more sophisticated model that considers both the overall strength of the board and specific constraints related to resources, health, and champion pool management. Adjust the formulation based on the specific details and dynamics of your TFT game.