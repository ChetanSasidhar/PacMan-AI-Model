
# Deep Convolutional Q-Learning for Pac-Man

This project implements a Deep Convolutional Q-Learning (DQN) agent to play the classic game Pac-Man using deep learning techniques. The project is structured in a step-by-step manner to build, train, and evaluate the AI model. The implementation leverages PyTorch for building neural networks and Gymnasium for the game environment.

## Overview

### Part 0: Installation and Setup
- **Packages**: The script installs necessary packages including Gymnasium and its dependencies, PyTorch, and other utility libraries.
- **Libraries**: Key libraries such as `numpy`, `torch`, `random`, and others are imported.

### Part 1: Neural Network Architecture
- **Network Class**: Defines a convolutional neural network with several layers including convolutional, batch normalization, and fully connected layers.
- **Forward Method**: Implements the forward pass of the network to process input states and produce action-value predictions.

### Part 2: Environment Setup
- **Gymnasium**: Initializes the Pac-Man environment using `MsPacmanDeterministic-v0` from Gymnasium.
- **State and Action Space**: Configures the state shape and action space for the environment.

### Part 3: Experience Replay and Agent
- **Replay Buffer**: Utilizes a deque to store experience tuples for training.
- **DQN Agent**: Implements the agent that interacts with the environment, updates policies, and uses experience replay for training.

### Part 4: Training and Evaluation
- **Training Loop**: Runs episodes to train the agent, including steps for action selection, state transition, reward handling, and network updates.
- **Evaluation**: Periodically evaluates the agent’s performance to monitor learning progress.

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your_username/deep_convolutional_q_learning_for_pac_man.git
   cd deep_convolutional_q_learning_for_pac_man
   ```

2. **Install Dependencies**:
   Ensure you have Python and pip installed, then run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Training Script**:
   Execute the script to start training the DQN agent:
   ```bash
   python deep_convolutional_q_learning_for_pac_man.py
   ```

## Requirements

- Python 3.x
- Gymnasium
- PyTorch
- NumPy
- Other dependencies as listed in `requirements.txt`

## Acknowledgments

- The implementation references the DQN algorithm and best practices from deep reinforcement learning research.
- Gymnasium for providing the game environment and tools.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.


