# Minesweeper Game with AI

A graphical Minesweeper game implementation in Python with an integrated AI agent that can solve the game.

## Prerequisites

- Python 3.x
- pip (Python package manager)

## Installation

1. **Install required dependencies:**

```bash
pip install -r requirements.txt
```

This will install:
- `pygame` - The graphics library used for the game interface

## Running the Program

To start the game, run:

```bash
python runner.py
```

The game window will open with an 8x8 Minesweeper board containing 8 mines.

## How to Play

### Game Rules
- The board is 8x8 with 8 randomly placed mines
- Click on cells to reveal them
- A number indicates how many mines are adjacent to that cell
- Flag cells you suspect contain mines
- Win by revealing all non-mine cells
- Lose if you reveal a cell with a mine

### Controls
- **Left Click**: Reveal a cell
- **Right Click**: Flag/unflag a cell as a mine
- **AI Button**: Let the AI solve the game automatically
- **Reset Button**: Start a new game

## Project Structure

```
minesweeper/
├── runner.py           # Main game runner and GUI
├── minesweeper.py      # Core game logic and AI agent
├── requirements.txt    # Project dependencies
├── assets/
│   ├── fonts/         # Game fonts
│   └── images/        # Game images (flags, mines)
└── README.md          # This file
```

## Game Configuration

You can modify the game settings in `runner.py`:

- `HEIGHT = 8` - Board height
- `WIDTH = 8` - Board width  
- `MINES = 8` - Number of mines on the board

## Features

- **Interactive GUI** using Pygame
- **AI Agent** capable of solving Minesweeper using inference
- **Game Instructions** displayed at startup
- **Visual Feedback** with flags and mine indicators

## Troubleshooting

**Issue: "No module named 'pygame'"**
- Solution: Run `pip install pygame`

**Issue: Missing fonts or images**
- Ensure the `assets/` folder with `fonts/` and `images/` subdirectories exists in the project directory

## AI Algorithm

The AI agent uses logical inference to:
1. Identify safe cells to reveal
2. Determine which cells must contain mines
3. Make optimal moves based on sentence logic and constraint satisfaction

---

**Developed as part of CS50's Introduction to AI with Python**
