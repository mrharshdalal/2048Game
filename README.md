# 2048 Game in Java

![image](https://github.com/mrharshdalal/2048Game/assets/64740456/3e0a5902-9368-49d0-bde7-108f5cb4c98b)


## Description

This is a Java implementation of the classic 2048 puzzle game. The goal of the game is to merge tiles with the same number to reach the coveted 2048 tile. It's a simple yet addictive game that you can play on your desktop.

## How to Play

- Use the arrow keys (Up, Down, Left, Right) to move the tiles on the grid.
- Tiles with the same number will merge into a single tile with a higher number when they collide.
- The game is won when you reach the 2048 tile.
- The game is lost when the grid is full, and you can no longer make a move.

## Features

- Simple and intuitive user interface.
- Keyboard controls for easy tile movement.
- Keeps track of your current score.
- Win and lose conditions for a challenging gameplay experience.

## Algorithm and Game Logic

### Game Logic Overview

1. **Initialization**: When the game starts, it initializes the game board, sets the initial score to zero, and adds two random tiles (either 2 or 4) to the board.

2. **User Input**: The player interacts with the game using arrow keys (Up, Down, Left, Right) to move the tiles on the grid.

3. **Tile Movement**: When the player presses an arrow key, the game attempts to move the tiles in that direction. Tiles with the same value merge into one if they collide during the move.

4. **Merging Tiles**: When two tiles with the same value collide, they merge into a single tile with a value equal to the sum of their values. This contributes to the player's score.

5. **Winning Condition**: The player wins the game when they reach the 2048 tile.

6. **Losing Condition**: The game is lost when there are no valid moves left, and the grid is full.

### Key Functions and Algorithms

Here are some of the key functions and algorithms used in your code to achieve the game's logic:

- `resetGame()`: Initializes the game board, score, and adds the first two tiles.
- `left()`, `right()`, `up()`, `down()`: Handle tile movement in different directions by applying rotation and then moving tiles to the left.
- `tileAt(x, y)`: Retrieves the tile at a specific (x, y) position on the grid.
- `addTile()`: Adds a new tile (2 or 4) to an empty spot on the grid.
- `availableSpace()`: Identifies and returns a list of available empty spots on the grid.
- `isFull()`: Checks if the grid is full (no empty spots).
- `canMove()`: Determines if any valid moves are left on the grid.
- `compare()`: Compares two lines of tiles to check if they are equal.
- `rotate()`: Rotates the entire grid by 90, 180, or 270 degrees.
- `moveLine()`: Shifts non-empty tiles in a line to the left.
- `mergeLine()`: Merges tiles in a line if they have the same value.
- `getLine()` and `setLine()`: Get and set a line of tiles in a specified direction.
- `drawTile()`: Renders tiles with appropriate colors and values on the game board.
- `offsetColors()`: Calculates the offset for drawing tiles.

You can describe these functions and algorithms in more detail in your README file. Additionally, you can provide code comments explaining how each function works within your Java code for those interested in a deeper understanding of your game's implementation.

## Getting Started

### Prerequisites

Make sure you have the following installed on your system:

- Java Development Kit (JDK) 8 or higher
- Git (optional)

### Installation

1. Clone the repository (if you haven't already):

   ```bash
   git clone https://github.com/mrharshdalal/2048-game-java.git
