# Pacman Q-Learning Agent (Reinforcement Learning)

> A tabular Q-learning agent built from scratch that learns to play Pacman purely from reward signals.

🔒 **The source code is in a private repository** because this was university coursework at King's College London. I'm happy to walk through the code on request.

## Overview
I implemented an online reinforcement-learning agent on top of the UC Berkeley Pacman framework. It learns a state–action value function Q(s, a) during play. It wins at least 8 out of 10 games on the smallGrid layout after 2,000 training episodes, and it also runs reliably on other layouts.

## What I built
- **Compact state representation:** a hashable feature wrapper based on Pacman's position, ghost positions and the food layout
- **Reward shaping:** penalties for being next to a ghost, rewards for food, and a small step cost that encourages efficient paths
- **Q-learning update:** online temporal-difference updates with a configurable learning rate and discount factor
- **Count-based exploration:** an exploration function that favours actions that have rarely been tried (optimism in the face of uncertainty), rather than plain ε-greedy
- **Training lifecycle:** the policy is automatically frozen once training finishes, and the hyperparameters can be set from the command line

## Skills demonstrated
Reinforcement learning · algorithm implementation from first principles · reward design · experimentation

## Tech stack
Python (no ML libraries: everything implemented from scratch)
