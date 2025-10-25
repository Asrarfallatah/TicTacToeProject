# TicTacToeProject

## Overview
This project is a simple **Tic Tac Toe** game built in **Java**.  
It allows two players to play alternately and displays the game board in the console.  
The goal is to practice **2D arrays**, **loops**,  **meathods**, and **conditional logic** in Java.

---

## Features
- Two-player mode (Player X and computer O)
- Input validation (no overwriting existing moves)
- Checks for win and draw conditions
- Clear console board display using 2D arrays
- Modular structure for easy improvements

---

## Project Structure
TicTacToeProject/
│
├── src/
│ └── main/java/org/example/Main.java # Main game code
│
├── pom.xml # Maven configuration file (if used)
└── README.md # Project documentation

---

## How to Run the Project

### Option 1 — Using an IDE
1. Open the project in **IntelliJ IDEA** or **Eclipse**.  
2. Locate the file:
   src/main/java/org/example/Main.java
3. Click **Run ** to start the game.

### Option 2 — Using Command Line
1. Compile the program:
```bash
javac src/main/java/org/example/Main.java
2.Run it:
java org.example.Main


---

### How It Works

The game board is represented using a 2D String array.
Players take turns choosing a row and column number.
The program checks for:
Three in a row (horizontal)
Three in a column (vertical)
Diagonal win
The game ends when there’s a winner or the board is full.

---

### Future Improvements
make the CPU smarter 
Create a graphical interface using JavaFX

---

Asrar Fallatah
October 2025
