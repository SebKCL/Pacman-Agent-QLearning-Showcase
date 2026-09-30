# Pacman Q-Learning Agent (Reinforcement Learning)

> I wrote a tabular Q-learning agent from scratch that teaches itself Pacman from rewards alone.

🔒 The code sits in a private repository because this was King's College London coursework. Ask me and I'll walk you through it.

## Overview
The agent runs on the UC Berkeley Pacman framework and learns a value for each state and action, Q(s, a), as it plays. After 2,000 training games it wins at least 8 of 10 on smallGrid, and it handles other layouts too.

## What I built
- **State representation:** a hashable wrapper built from Pacman's position, the ghosts' positions and the remaining food
- **Reward shaping:** a penalty next to a ghost, a reward for food, and a small cost per step so Pacman takes short routes
- **Q-learning update:** temporal-difference updates on every move, with a tunable learning rate and discount factor
- **Exploration:** a count-based bonus that pushes Pacman towards the moves it has tried least, in place of plain ε-greedy
- **Training control:** the agent freezes its policy when training ends, and you can set every hyperparameter from the command line

## Skills
Reinforcement learning · algorithms from first principles · reward design · experimentation

## Tech stack
Python, with no ML libraries
