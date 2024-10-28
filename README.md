# Current-Emerging-Trends

## Project Overview: Intelligent Agent for Pathfinding

## Work Done on This Project - # I did NOT Write any of the files I contributed to the completion of the jupiter notebook file

In this project, I focused on developing an intelligent agent using deep Q-learning to navigate a maze and efficiently find the treasure.

### Given Code vs. Created Code

- **Given Code**: I received the foundational framework for the maze environment, including methods for observing the environment and handling actions, as well as the structure for managing agent interactions.

- **Created Code**: I implemented the following key components:

    - **Epoch Loop**: I created a loop to run multiple training epochs, where the agent attempts to navigate the maze and improve its performance.
    
    - **Agent Initialization**: The agent is randomly placed in a free cell within the maze using `agent_cell = qmaze.free_cells[np.random.randint(0, len(qmaze.free_cells))]` and reset to this position.
    
    - **State Observation**: I utilized the `observe` method to retrieve the current state of the maze.
    
    - **Action Selection**: The agent selects actions based on an exploration-exploitation strategy. It randomly chooses an action with probability `epsilon` (exploration) or selects the best-known action based on the Q-values (exploitation).
    
    - **Action Execution**: I implemented the mechanism to perform the chosen action and receive feedback in the form of the new state and reward.
    
    - **Experience Replay**: I stored episodes of the agent's experience using the `remember` method, allowing the model to learn from past interactions.
    
    - **Model Training**: I trained the neural network by calling `model.fit()` on the training data retrieved from the experience replay, iterating this process to refine the agent’s policy.

## Learning Connections

### The Role of Computer Scientists

Computer scientists design algorithms and systems that solve complex problems using computational methods. In artificial intelligence (AI), they develop models like neural networks and reinforcement learning agents that learn from data and adapt their behaviors. This work is crucial as it drives innovation across various industries, improving efficiency and enabling new technologies.

### Approach to Problem Solving

As a computer scientist, my approach to problem-solving includes:

1. **Define the Problem**: Clearly articulate the goal, such as guiding an agent to the treasure in the maze.
2. **Research Algorithms**: Explore relevant reinforcement learning algorithms, particularly Q-learning and experience replay.
3. **Design the Solution**: Architect the learning process for the agent, balancing exploration and exploitation effectively.
4. **Implement and Iterate**: Code the solution, test its performance, and refine based on outcomes and win rates.

### Ethical Responsibilities

My ethical responsibilities to the end user and the organization include:

- **User Privacy**: Ensuring that any data handled by the agent is protected and treated confidentially.
- **Transparency**: Clearly explaining how the agent makes decisions and learns from its environment, fostering user trust.
- **Safety and Fairness**: Ensuring the agent operates predictably and does not lead to biased outcomes.
- **Quality Assurance**: Delivering a reliable and efficient product that meets user needs effectively.

In summary, this project demonstrates the application of deep Q-learning for pathfinding while emphasizing the importance of ethical considerations in the development of intelligent agents.
