# Qualitative results
Here we can observe 5 execution of the agents trained with each RL algorithm (Q-learning, DQN, DDQN and A2C).

### Random agent
Example of a random agent sampling actions uniformly, just to set a behavior baseline of a non-trained agent.

![Alt Text](imgs/random/random.gif)

## Q-learning
The agent learns to fly and control the lander but find it difficult to land on the target position, probably due to discretization process of the state representations to estimate the table *Q[s,a]*.

![Alt Text](imgs/Q-learning/ql.gif)

## DQN
With DQN we begin to notice a great performance in landing the spacecraft to the target position.

![Alt Text](imgs/DQN/dqn.gif)

## DDQN
DDQN shows similar qualitative results as DNQ, although it appears to reach faster training convergence.

![Alt Text](imgs/DDQN/ddqn.gif)

## A2C
The A2C agent is able to control the lander perfectly and rapidly drives it carefully to the surface. However, it starts "jumping" instead of turning off the engine and finish the episode. Maybe this can be explained due to the short-sighted nature of the implemented algorithm (*n*-steps strategy). The agent discovers that each time the lander leg touches the ground it gets +10 of reward, so it continues jumping to earn extra short-term rewards.

![Alt Text](imgs/a2c/a2c_rare.gif)
