
# Connect 4 Game with Minimax Algorithm

## Overview

This project is a Connect 4 game implemented in Java, featuring an AI opponent using the Minimax algorithm with alpha-beta pruning. The game includes different levels of difficulty, including a stochastic level where the AI makes some moves randomly.

## Features

- **Single-player Mode**: Play against the AI.
- **Minimax Algorithm**: AI decision-making with alpha-beta pruning for efficiency.
- **Difficulty Levels**:
  - **Easy**: Random moves.
  - **Medium**: Limited depth minimax.
  - **Hard**: Full depth minimax with alpha-beta pruning.
  - **Stochastic**: Mix of minimax and random moves.
- **Undo Move**: Ability to undo the last move.

## Installation

To set up the Connect 4 game on your local machine, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/connect4-minimax.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd connect4-minimax
    ```

4. **Build and run the application**:
    - Using Maven:
        ```bash
        mvn clean install
        mvn exec:java -Dexec.mainClass="com.example.connect4.Connect4Game"
        ```
    - Using Gradle:
        ```bash
        gradle build
        gradle run
        ```

## Usage

### GUI Interface

- **Main Menu**: Select the difficulty level and start a new game.
- **Game Board**: Click on a column to place your piece. The AI will automatically make its move after yours.

### Difficulty Levels

- **Easy**: AI makes completely random moves.
- **Medium**: AI uses minimax with a limited search depth.
- **Hard**: AI uses full depth minimax with alpha-beta pruning for optimal moves.
- you can type the level from 1 to 7 
- **Stochastic**: AI uses a combination of minimax and random moves for unpredictability.

## Code Structure

- **src/main/java**: Contains the Java source code.
  - **com.example.connect4**: Main package containing core functionality.
    - **Connect4Game.py**: Main class to run the application.
    - **GameBoard.py**: Manages the game board state.
    - **MinimaxAI.py**: Implements the minimax algorithm with alpha-beta pruning.
    - **RandomAI.py**: Implements the random move generator for easy level.
    - **StochasticAI.py**: Combines minimax and random moves for the stochastic level.
    - **Move.java**: Represents a move in the game.


## Minimax Algorithm

The Minimax algorithm is used to determine the optimal move for the AI. Alpha-beta pruning is implemented to improve the efficiency of the search process by eliminating branches that do not need to be explored. The stochastic level introduces randomness to some moves to add unpredictability.

