# Reinforcement Learning OpenAI Gym

This project implements 2 reinforcement learning approaches (Deep Q-Learning and TD3) on the environments provided by OpenAI Gym
and introduces 3 tricks trying to further improve the base algorithms.

## Context
File name ended with "base" = Only base algorithm (DQN/TD3)\
File name ended with "1"    = Only semi-adaptive batch size is implemented in the base algorithm\
File name ended with "123"  = All 3 proposed methods are implemented in the base algorithm


## Results (in number of episodes)
|                  | Cart Pole | Mountain Car | Lunar Lander | Lunar Lander Continuous |
|------------------|-----------|--------------|--------------|-------------------------|
| Base             | 275.4     | 641.9        | 402.2        | 377.6                   |
| Base + 1         | 168.9     | 494.6        | 330.1        | 297.11                  |
| Base + 2         | 150.5     | 601.5        | 341.1        | -                       |
| Base + 3         | 130.2     | 600.5        | 366.0        | -                       |
| Base + 1 + 2     | 163.1     | 501.5        | 363.2        | -                       |
| Base + 1 + 3     | 148.9     | 606.4        | 354.2        | -                       |
| Base + 2 + 3     | 145.5     | 492.2        | 276.1        | -                       |
| Base + 1 + 2 + 3 | 137.6     | 723.9        | 309.3        | -                       |

## Acknowledgement
Code in CarPole-v0, MountainCar-v0, LunarLander-v2 are modified from\
https://github.com/hangsz/reinforcement_learning/tree/master/DQN/CartPole-v0

Code in LunarLanderContinuous-v2 is modified from\
https://github.com/nikhilbarhate99/TD3-PyTorch-BipedalWalker-v2
