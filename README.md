# Tic-Tac-Toe Project

## Overview
This project is a console-based **Tic-Tac-Toe** game built in **Java** (JDK 8+). It features a single-player mode where you compete against a **randomized CPU opponent**. The game manages multiple rounds and calculates a final score summary.

This implementation served as a practical exercise to reinforce core Java concepts, including:
* **2D Arrays** for complex board representation.
* **Methods** for modular code design (e.g., `winnerCheck`, `isPlaceAvailable`).
* **Input Handling** with robust **`try-catch`** blocks to manage errors.
* **Conditional Logic** for game rules, validation, and turn management.

---

## Features
* **Single-Player Mode:** Play as 'X' against the Computer 'O'.
* **Multi-Round Play:** The user specifies the total number of rounds to play at the start.
* **Robust Input Validation:** Handles invalid input (non-integers, numbers out of range) and checks for spot availability.
* **Win/Draw Detection:** Accurately checks for all horizontal, vertical, and diagonal win conditions.
* **Score Summary:** Prints the final tally of Player Wins, CPU Wins, and Ties.

---

## Project Structure
TicTacToeProject/ 
│ ├── src/ │ └── main/java/org/example/Main.java # Contains all game logic and the main execution method. 
│ ├── pom.xml # Standard Maven configuration file.
└── README.md # Project documentation

---

## How to Run the Project

### Option 1 — Using a Java IDE (Recommended)
1.  Clone the repository and open the project in your preferred IDE (**IntelliJ IDEA**, **Eclipse**, or **VS Code** with Java extensions).
2.  Navigate to the main class: `src/main/java/org/example/Main.java`.
3.  Click the **Run** button (usually a green triangle) to compile and start the game.

### Option 2 — Using Command Line
Assuming you have the Java Development Kit (JDK) installed and are in the root `TicTacToeProject/` directory:

1.  **Compile** the source code:
    ```bash
    javac src/main/java/org/example/Main.java
    ```
2.  **Run** the compiled program:
    ```bash
    java org.example.Main
    ```
    The console will immediately prompt you to enter the number of rounds you wish to play.

---

## Core Logic Highlights

| Concept | Implementation Detail |
| :--- | :--- |
| **Board Structure** | A **7x7 2D `String` array** is used, where inner elements (`|`, `+`, `--`) form the visual grid, and positions are mapped to non-consecutive indices (e.g., choice 1 is `[1][1]`). |
| **Move Mapping** | Player input (1-9) is translated into the correct `[row][column]` array indices using a long series of `if/else if` statements within `playerDesitions` and `cpuDesitions`. |
| **CPU Strategy** | The CPU uses the `Random` class to select a move and continuously retries (`do-while` loop) until a valid, **available** spot is found. |
| **Game Flow** | The main loop manages turns, calls the `playerDesitions` and `cpuDesitions` methods, and immediately checks for a winner or a draw after each move. |

---

## Future Improvements
* **Advanced CPU:** Replace the random CPU logic with an intelligent algorithm (e.g., **Minimax**) to create an unbeatable opponent.
* **GUI Interface:** Develop a graphical user interface using **JavaFX** or **Swing** to replace the console output.

---
Developed by
**Asrar Fallatah** | **October 2025**
