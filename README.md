# Pacman-AI
Note: Code is kept private, can show on a need-to-know basis. Attributed to UC Berkeley (http://ai.berkeley.edu)

This project implements various search algorithms that takes Pacman to the goal state. 

For Single-Agent Pacman:
1. Iterative Deepening: The iterativeDeepeningSearch function in search.py is an interative-deepening search algorithm that takes a search problem as input and  returns a plan (list of actions) that takes Pacman to the goal state.
2. A* Search: The aStarSearch function in search.py is an A* search algorithm that takes a search problem and heuristic as input and returns a plan (list of actions) that takes Pacman to the goal state.


For Multi-Agent Pacman:

An evaluation function is implemented that returns a higher number for a better state and/or action, and a lower number for a worse state. It considers both the food location and ghost locations to perform well.
1. Minimax: The search agent uses minimax to select which action Pacman will take. This works with any number of ghosts since the minimax tree has multiple min layers (one for each ghost) for every max layer. If a state is a leaf, the value returned by the evaluation function mentioned above is returned.
2. Expectimax: Minimax assumes the adversary makes optimal decisions, which might not be the case. The expectimax search agent takes the expected value according to its model of how the ghosts act.
