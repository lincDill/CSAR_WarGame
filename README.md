# CSAR_WarGame
A Python-based digital implementation of a cooperative Combat Search and Rescue (CSAR) tabletop wargame originally developed as part of a military wargaming course.
The game places four players in different CSAR role working together to recover an isolated personnel (IP) member while overcoming enemy threats, degraded communications, and mission setbacks.

## Player Roles
The game includes four player roles:
- **Strike**
- **C2**
- **Escort**
- **Rescue**
  
Each role has its own deck of cards representing different capabilities. At the beginning of the game, each player selects a five-card loadout.

## Objective
Players must successfully complete four increasingly difficult mission phases (based on the phases of a CSAR mission) and reach the IP.
Each phase introduces enemy threats that must be defeated using the team's available cards and effects.

## Basic Rules
1. Each player begins with a five-card loadout.
2. Players take turns playing one card from their hand.
3. Cards may:
       - Attack enemy threats
       - apply special effects
       - Support other player cards
       - Perform both an attack and an effect
4. Threats may begin face-down, creating uncertainty about their strength or type.
5. Attacks are affected by the compatibility between a player's capability and the threat category.
6. Damage to threats is cumulative across player actions.
7. Some threats produce effects rather than having a traditional strength value.
8. Once all required threats in a phase are defeated, the team advances to the next phase.
9. If the ream fails a phase, a **Setback Card** is drawn and the phase must be attempted again.
10. Accumulating too many setbacks results in mission failure.
11. Between phases, an **IP Card** is drawn to represent the actions of the IP
12. The "Authentication Success" **IP Card** must be drawn to rescue the IP and win the game. This card remains active for the remainder of the game when drawn.

## Fog of War
The original tabletop version includes a communication restriction designed to simulate radio jamming and operational friction.
During mission execution (the actual gameplay during the phase), players cannot communicate. Coordination is allowed only between phases during structured mission brief and after-action-review periods.
This mechanic forces players to anticipate the actions of other team members rather than perfectly coordinating every move.

# Mission Progression
The game contains four phases, with the number of threats increasing as the team approaches the IP:
  | Phase | Threats |
  |-------|---------|
  |   1   |    3    |
  |   2   |    4    |
  |   3   |    5    |
  |   4   |    6    |
  
Threats include categories such as:
- Surface-to-Air Missile (SAM)
- Air
- Ground
- Electronic Warfare (EW)
Additional threat and setback effects can modify the battlefield throughout the mission.
Between phases, IP cards add randomness from the IP side of the scenario, representing factors such as compliance with survival/evasion procedures and possession of authenticated credentials.

# Winning and Losing
**Win:** Successfully complete all four phases and recover the IP.
**Loss:** Accumulate more than 5 **Setback Cards** to cause mission failure.

## Project Purpose
This project converts the original tabletop wargame into a playable Python environment while preserving its cooperative decision-making, uncertainty, card interactions, and operational friction.
A separate reinforcement learning version of the project is also being developed to explore autonomous decision-making, strategy discovery, balance testing, and AI-assisted wargaming.

## Status
This project is actively being developed. Core gameplay, card interaction, phase progression, threats, setbacks, and automated effects are implemented, with additional card effects and balancing improvements continuing to be added.
