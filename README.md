# Unsupervised and Reinforcement Learning
Unsupervised and Reinforcement Learning (URL) assignments for Master in Artificial Intelligence @ UPC.

## Unsupervised Learning
Analysis of Power Iteration Clustering, a spectral clustering algorithm which is a simple, fast and effective approach for finding data clusters based on spectral properties of affinity matrices:

<img src="Unsupervised Learning/figs/pic-crop.gif"/>

## Reinforcement Learning

Analysis of different RL algorithms (Q-learning, DQN, DDQN and A2C) on OpenAI gym framework.

### Random agent
Example of a random agent sampling actions uniformly, just to set a behavior baseline of a non-trained agent.

<img src="Reinforcement Learning/FinalProject/imgs/random/random.gif" style="width:50%"/>

## Q-learning
The agent learns to fly and control the lander but find it difficult to land on the target position, probably due to discretization process of the state representations to estimate the table *Q[s,a]*.

<img src="Reinforcement Learning/FinalProject/imgs/Q-learning/ql.gif" style="width:50%"/>

## DQN
With DQN we begin to notice a great performance in landing the spacecraft to the target position.

<img src="Reinforcement Learning/FinalProject/imgs/DQN/dqn.gif" style="width:50%"/>

## DDQN
DDQN shows similar qualitative results as DNQ, although it appears to reach faster training convergence.

<img src="Reinforcement Learning/FinalProject/imgs/DDQN/ddqn.gif" style="width:50%"/>

## A2C
The A2C agent is able to control the lander perfectly and rapidly drives it carefully to the surface. However, it starts "jumping" instead of turning off the engine and finish the episode. Maybe this can be explained due to the short-sighted nature of the implemented algorithm (*n*-steps strategy). The agent discovers that each time the lander leg touches the ground it gets +10 of reward, so it continues jumping to earn extra short-term rewards.

<img src="Reinforcement Learning/FinalProject/imgs/a2c/a2c_rare.gif" style="width:50%"/>
