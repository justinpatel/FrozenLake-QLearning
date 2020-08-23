# FrozenLake-QLearning
Creating a Q table for a frozen-lake problem using Reinforcement Learning

Used gym toolkit from openai

5 Important things for Reinforcement Learning:
1. Environment
2. Agent
3. States
4. Action
5. Reward

This is the equation to feed values in Qtable:     
```Q[state, action] = Q[state, action] + LEARNING_RATE * (reward + GAMMA * np.max(Q[next_state, :]) - Q[state, action])```


