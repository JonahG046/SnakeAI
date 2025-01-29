# Snake AI with Deep Q-Learning

This project is a Python implementation of a Snake game where the AI learns to play using Deep Q-Learning. The AI agent is trained to maximize its score by exploring the game environment, and learning optimal moves through reward-based training. The model is built using PyTorch.

## Requirements:
- Python 3.x
- `pygame` for game visualization
- `torch` for building and training the neural network model
- `numpy` for array manipulation
- `matplotlib` for plotting training results

You can install the necessary libraries using the following command:

```bash
pip install pygame torch numpy matplotlib
```

## How To Run

Run the training script to train the AI:

```bash
python train.py
```

this script initializes the game environment, trains the AI using Deep Q-Learning, and plots the training results.
## Files and Usage
- **SnakeGame.py**: Defines the `SnakeGameAI` class that handles mechanics and logic, including movement, collision detection, and scoring.
- **model.py**: Contains the neural network (`Linear_QNet`) used to approximate the Q-function and the `QTrainer` class for training the model using gradient descent.
- **helper.py**: Provides a plotting function (`plot`) to visualize the game scores and mean scores during training.
- **train.py**: Implements the reinforcement learning training loop where the AI learns to improve its gameplay.

## Customization

- Adjust `BLOCK_SIZE`, `SPEED`, and other parameters in `SnakeGameAI.py` to modify game behavior and performance.
- Modify the neural network architecture (`Linear_QNet`) in `model.py` to experiment with different network configurations for better performance.

  ## Training and Results

 The AI agent learns from playing the game autonomously and improves its strategy over time using Deep Q-Learning. Training progress is visualized using Matplotlib, showing the scores obtained per game and the mean scores over multiple games.

 ## License 

 This project is licensed under the MIT License - see the [MIT License](LICENSE) file for details.







