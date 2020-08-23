# FrozenLake-QLearning 🕹
## Creating a Q table for a frozen-lake problem using Reinforcement Learning

Used openai's gym toolkit

> 5 Important things for Reinforcement Learning:
> 1. Environment 🎮
> 2. Agent 👤
> 3. States 🎰
> 4. Action 🎲
> 5. Reward 🥇

Environment of FrozenLake problem: <br />
SFFF <br />
FHFH <br />
FFFH <br />
HFFG <br />

- S stands for Starting position, safe
- F stands for frozen lake which is walkable, safe
- H stands for Hole in frozen lake, fail
- G stands for Goal

> The Agent will explore the different ways to reach the goal and is rewarded for finding a walkable path to a goal. 

This is the equation to feed values in Qtable:     
`Q[state, action] = Q[state, action] + LEARNING_RATE * (reward + GAMMA * np.max(Q[next_state, :]) - Q[state, action])`

> Qtable contains the transitional values of between states and action.
