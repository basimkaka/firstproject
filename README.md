# Bumpers Car Collision Game

A JavaFX-based game where cars move around a game board, avoiding collisions. The player controls a fast car, while autonomous slow cars roam the board. Collisions are detected, and the winner is determined based on position.

## Features
- **Player-controlled car**: Use the toolbar to start/stop the game and control the speed.
- **Autonomous cars**: Multiple slow cars move randomly on the board.
- **Collision detection**: Determines which car wins when a collision occurs.
- **Audio effects**: Background music and crash sounds (requires implementation of `AudioPlayerInterface`).
- **Dynamic movement**: Cars bounce off the board boundaries.

## Requirements
- **Java 11 or higher** (JavaFX is required).
- **JavaFX SDK** (version 17 or compatible).
- Maven/Gradle (optional, for dependency management).

## Project Structure
Key classes and their responsibilities:
- `BumpersApplication`: Main JavaFX application entry point.
- `GameBoard`: Manages game logic, cars, and collisions.
- `Car`: Abstract class for car behavior. Extended by `FastCar` (player) and `SlowCar`.
- `Player`: Represents the player and their car.
- `Collision`: Handles collision detection and winner evaluation.
- `GameBoardUI`: Renders the game board and cars using JavaFX.
- `GameToolBar`: Provides UI controls (start/stop buttons).

## Setup and Run
### Using an IDE (e.g., IntelliJ/Eclipse):
1. **Ensure JavaFX is configured** in your IDE. Add VM options for JavaFX modules:
2. **Run `Bumpers.java`** as the main class.

### Command Line (with Java 11+):

How to Play
Start the game: Click the "Start" button in the toolbar.

Control speed: Use the toolbar buttons to increment/decrement the player car's speed.

Avoid collisions: If a collision occurs, the car positioned farther right wins.

Stop the game: Click the "Stop" button to halt all movement.

Notes
Ensure image files (FastCar.gif, SlowCar.gif) are placed in the correct resource directory.

Implement AudioPlayerInterface to enable sound effects (see GameBoard class).

License
This project is intended for educational purposes. Modify and use it according to your needs.