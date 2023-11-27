# ReinforcementLearningMCforBlackjack
General

In various reinforcement learning problems, we try to obtain the optimal policy by continuing to play the game and updating our predictions. Basically, the (situation, value) pair or (situation, action, value) pair is predicted and based on the predictions, the action that gives the highest value is taken, thus the policy is created.

In the Monte Carlo Method the idea is simple and intuitive; if we are unsure of the value of a state, we simply sample; this is to continue visiting that state and interacting with the environment, averaging out the reward from simulated actions.

Estimation

The simulation is run for 10,000 rounds and state-value predictions are generated.
Column z is the number of wins in that division. If a player's value is 20 or 21, he is more likely to win. In general, the policy here leads to high-loss situations. The chance of winning is around 30 percent.
![image](https://github.com/ozgurgeylani/ReinforcementLearningMCforBlackjack/assets/48389658/dddb31f4-06ba-462e-890b-6754b4629bb7)

It has also been observed that the available ace leads to good results depending on the nuances of playing the game. Based on the conclusion in Sutton's book, a usable ace increases his chances of winning, as a player with a usable ace has a higher chance of hitting. Even if the value goes above 21, it can continue, making the usable ace unusable.
![image](https://github.com/ozgurgeylani/ReinforcementLearningMCforBlackjack/assets/48389658/9dec9ff2-53cc-4edf-9b80-1dca619630fb)
