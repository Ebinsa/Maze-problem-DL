This project implements maze-solving algorithms using SARSA (State-Action-Reward-State-Action) and DQN (Deep Q-Network) reinforcement learning techniques. The goal is to navigate through a maze environment and learn optimal policies for efficient maze traversal.

Getting Started
Clone the Repository:
git clone https://github.com/your-username/maze-solver.git
cd maze-solver

Install Dependencies:
pip install -r requirements.txt

Maze Environment
The maze environment is represented as a grid, where each cell can be either open or blocked. The agent starts at a specified starting point and must navigate to the goal while avoiding obstacles.

SARSA Algorithm
Implementation
The SARSA algorithm is implemented in the sarsa.py file. The Q-values are updated based on the observed transitions using the SARSA update rule.
# Pseudocode for SARSA Update
Q[state][action] += alpha * (reward + gamma * Q[next_state][next_action] - Q[state][action])
python sarsa.py


DQN Algorithm
Implementation
The DQN algorithm is implemented in the dqn.py file. It utilizes a neural network to approximate the Q-values and experience replay for better training stability.

Configuration
You can configure various parameters such as learning rate, discount factor, exploration rate, neural network architecture, etc., in the config.py file.

Results
The trained agents' performance and learned policies will be saved in the results/ directory. You can visualize the results using appropriate visualization tools or by analyzing the saved data.

Contributing
Feel free to contribute by opening issues or submitting pull requests. If you have any ideas for improvements or find any bugs, please let us know!
