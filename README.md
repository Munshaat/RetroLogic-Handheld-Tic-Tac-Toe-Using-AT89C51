# RetroLogic Handheld Tic-Tac-Toe Using AT89C51

A microcontroller-based **Tic-Tac-Toe game** designed and simulated using the **AT89C51 (8051 family) microcontroller** in Proteus. The project combines keypad input, LCD-based display, game-state processing, and decision-making logic to create an interactive handheld-style game.

## Project Overview

The project implements a digital Tic-Tac-Toe game using an **AT89C51 microcontroller**, a **4×4 keypad**, and a **20×4 LCD**.

The system supports both:

* **Player vs Player (PvP)**
* **Player vs AI (PvAI)**

The AI mode includes decision-making logic for selecting moves based on the current game state.

## Key Features

* AT89C51-based embedded game system
* 4×4 keypad for user input
* 20×4 LCD for game display
* Player vs Player mode
* Player vs AI mode
* Winning-move detection
* Blocking opponent's winning move
* Fork detection
* Corner and side move selection
* Game-state processing
* Proteus circuit simulation

## Hardware Components

* AT89C51 Microcontroller
* 4×4 Matrix Keypad
* 20×4 LCD
* Crystal oscillator
* Resistors and capacitors
* Power supply circuitry
* Supporting interfacing components

## Game Architecture

```text
          4×4 Keypad
               │
               ▼
        ┌──────────────┐
        │   AT89C51    │
        │ Microcontroller│
        └──────┬───────┘
               │
       ┌───────┴────────┐
       ▼                ▼
  Game Processing    AI Decision
       │                │
       └───────┬────────┘
               ▼
           20×4 LCD
               │
               ▼
          Game Display
```

## Game Modes

### Player vs Player

Two players take turns selecting positions on the board using the keypad.

The microcontroller:

1. Accepts the player's keypad input.
2. Updates the game state.
3. Displays the updated board.
4. Checks for a winning condition.
5. Checks whether the game has ended in a draw.
6. Switches to the next player's turn when appropriate.

### Player vs AI

In AI mode, the microcontroller evaluates the current board before selecting its move.

The decision-making logic considers:

1. **Winning move** — checks whether the AI can win immediately.
2. **Blocking move** — checks whether the opponent can win on the next move.
3. **Fork opportunity** — considers moves that create multiple winning possibilities.
4. **Corner selection** — considers available corner positions.
5. **Side selection** — uses available side positions when appropriate.

This provides a rule-based AI opponent rather than relying on random movement.

## User Interface

The **4×4 keypad** is used to select game positions and interact with the system.

The **20×4 LCD** provides the visual interface for:

* Game board
* Player turns
* AI turns
* Game results
* User interaction

## Proteus Simulation

The complete circuit was designed and tested in **Proteus**.

Simulation was used to verify:

* Microcontroller operation
* Keypad input
* LCD interfacing
* Game-state transitions
* Player turns
* AI decisions
* Winning and draw conditions

## Software and Tools

* **Proteus**
* **AT89C51 / 8051 Microcontroller**
* **Embedded C / 8051 programming**
* Matrix keypad interfacing
* LCD interfacing

## Project Highlights

* Designed an interactive embedded Tic-Tac-Toe system.
* Implemented keypad-based user interaction.
* Interfaced a 20×4 LCD with the AT89C51.
* Developed PvP and PvAI game modes.
* Implemented rule-based AI decision making.
* Added winning and blocking strategies.
* Implemented fork, corner, and side selection logic.
* Verified the complete system through Proteus simulation.

## Repository Structure

```text
retrologic-tic-tac-toe-8051/
│
├── README.md
├── RetroLogic Handheld Tic-Tac-Toe Using AT89C51.pdf
│
├── Proteus/
│   └── [Proteus project files]
│
└── Code/
    └── [Microcontroller source files]
```

## Academic Project

**Department of Electrical and Electronic Engineering**
**Islamic University of Technology (IUT)**

**Project:** RetroLogic Handheld Tic-Tac-Toe Using AT89C51
