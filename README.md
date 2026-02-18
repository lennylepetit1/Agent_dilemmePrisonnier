# Agent_prisonner_dilemma

Our objective is to create an agent that learns to play the standard Prisoner’s Dilemma. Our agent uses a Q-learning algorithm to learn, with a decaying epsilon exploration rate over time.

In the first part of the code (“4premiers”), our agent plays against four different types of opponents:

AlwaysCooperate: this opponent always cooperates with us.

AlwaysDefect: this opponent always defects against us.

Tit-for-Tat: this opponent plays, at round N, the action that the player chose at round N−1.

Random: this opponent randomly chooses between cooperation and defection with probability 0.5 for each action.

The results are displayed in a graph that appears when running the “4premiers” code. The different learned strategies are stored in a memory structure called trained_agent_Qtable.

Next, we tested a final scenario in which our agent plays against a copy of itself. However, our agent updates its memory every 50 matches, while its opponent does not. We observe that our agent gradually outperforms its opponent over time. This code is contained in the section named “Duel.”
