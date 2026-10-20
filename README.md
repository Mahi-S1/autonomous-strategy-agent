# Autonomous Strategy Agent (NSUT AutoPilot)

Tournament agent implementation for the AutoPilot competition featuring a **Staggered Iron Wall & Focused Archer Battery** strategy.

## Key Strategy & Scoring Pillars

- **Guaranteed Win & 0 Defence Losses:** Staggered Shields placed across active rows (at `x = 3` for even rows, `x = 4` for odd rows). This geometry ensures a minimum Euclidean distance of $\approx 2.12$ units between adjacent row shields, completely isolating 2.0-unit Pirate explosion splash damage.
- **Wave Elimination (100% Kills):** Archer battery positioned at `x = 0` provides global focus fire across lanes, eliminating regenerators and high-threat units rapidly.
- **Direct-fire Soldier Support:** Placed at `x = 1` prioritized in lanes with Wizard (beam) and Pirate threats to eliminate targets before shields sustain critical wear.
- **Economy & Budget Optimization:** Disciplined spending logic preserves unspent coin reserves once active lanes are secured to maximize economy score.

## Project Structure

```
autonomous-strategy-agent/
├── agent.py       # Core tournament agent logic & get_reinforcements entry point
├── .gitignore     # Git ignore rules
└── README.md      # Strategy & project documentation
```
