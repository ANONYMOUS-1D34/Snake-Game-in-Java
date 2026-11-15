# Java Snake Game

A classic Snake game built in **Java** using **Java Swing** and **AWT**. Control the snake with the arrow keys, eat apples to grow longer and increase your score, and avoid hitting the walls or your own body.

## Features

- Classic grid-based Snake gameplay.
- Keyboard controls using the arrow keys.
- Random apple placement on the game grid.
- Snake grows and the score increases whenever an apple is eaten.
- Collision detection for the game boundaries and the snake's own body.
- Simple graphical interface with a black background, green snake, red apples, and a score display.

## Requirements

- Java Development Kit (JDK) installed.
- A desktop environment that supports Java Swing (the game opens a graphical window).

The project uses Java's built-in Swing, AWT, and `java.util.Random` libraries. No external dependencies or build tools are required.

## How to Run

1. Clone or download this repository.
2. Open a terminal in the folder containing `SnakeGame.java`.
3. Compile the source file:

   ```bash
   javac SnakeGame.java
   ```

4. Start the game:

   ```bash
   java SnakeGame
   ```

## Controls

| Key | Action |
| --- | --- |
| `↑` Up Arrow | Move up |
| `↓` Down Arrow | Move down |
| `←` Left Arrow | Move left |
| `→` Right Arrow | Move right |

The game prevents the snake from immediately reversing into the opposite direction.

## How to Play

- The snake starts with six segments and initially moves to the right.
- Guide it toward the red apple.
- Each apple eaten increases the score by one and makes the snake longer.
- Avoid the edges of the game window and the snake's own body. Either collision ends the game.
- The final score is shown on the Game Over screen.

## Project Structure

```text
Java-Snake-Game/
├── SnakeGame.java   # Main window, game panel, gameplay logic, and keyboard input
└── README.md        # Project documentation
```

## Technical Overview

- **`SnakeGame`** extends `JFrame` and creates the game window.
- **`GamePanel`** extends `JPanel` and contains the game state, drawing logic, movement, apple handling, collision checks, and timer-based updates.
- **`MyKeyAdapter`** handles arrow-key input and changes the snake's direction.
- A Swing `Timer` updates the game approximately every 75 milliseconds.

## Contributors

- Daniyal Riaz

Made as a Java OOP lab project.
