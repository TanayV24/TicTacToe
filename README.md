<div align="center">

# 🎮 TicTacToe

### Classic Tic-Tac-Toe Game — Two-Player (or optional AI) on 3×3 Grid

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/Tkinter-GUI-FF6F00?style=for-the-badge)
![Game](https://img.shields.io/badge/Game-TicTacToe-blue?style=for-the-badge)

**A simple and interactive Tic-Tac-Toe game implemented in Python (with GUI), allowing two players to play, with full game logic including win/draw detection and option to restart.**

[📖 Documentation](#features) | [🐛 Report Bug](https://github.com/TanayV24/TicTacToe/issues) | [💡 Request Feature](https://github.com/TanayV24/TicTacToe/issues)

</div>

---

## ✨ Features

- 🎯 **Classic 3×3 Board** — Standard Tic-Tac-Toe layout and rules (X vs O). :contentReference[oaicite:1]{index=1}  
- 🔄 **Player Turns** — Players alternate turns; valid move enforcement prevents overwriting moves. :contentReference[oaicite:2]{index=2}  
- ✅ **Win Detection** — Automatically detects win when a row, column, or diagonal is filled by same symbol. :contentReference[oaicite:3]{index=3}  
- 🤝 **Draw Detection** — If all cells are filled without a winner, declares a tie/draw. :contentReference[oaicite:4]{index=4}  
- 🔁 **Restart / New Game** — Allows players to reset the board and play again. :contentReference[oaicite:5]{index=5}  
- 🖥️ **GUI Interface (Tkinter or equivalent)** — Buttons grid for board, user-friendly interaction. :contentReference[oaicite:6]{index=6}  

---

## 🛠 Tech Stack

| Layer       | Technology                  |
|------------|-----------------------------|
| Language   | Python 3.8+                 |
| GUI / UI   | Tkinter (or chosen GUI lib) |
| Logic      | Plain Python / OOP          |
| Tools      | Standard Python libraries   |

---

## 📋 Prerequisites

- 🐍 Python 3.8 or above  
- (If GUI) Tkinter — comes bundled with standard Python installs  
- 💻 Git (optional, for version control)  

Verify installation:

```bash
python --version
````

---

## ⚙️ Installation & Setup

### 🚀 Quick Start

```bash
git clone https://github.com/TanayV24/TicTacToe.git
cd TicTacToe
python main.py     # or whichever is your entry script (e.g. tic_tac_toe.py)
```

If using a GUI, window should open directly; if console version, follow prompts.

---

## 🎮 How to Play

1. Launch the game
2. Players take turns placing “X” or “O” in empty grid cells
3. Once a player gets three in a row (horizontal / vertical / diagonal), the game shows winner
4. If board fills up without a winner — it’s a draw
5. Choose “Restart / New Game” to play again

---

## 📁 Project Structure (Detailed)

```
TicTacToe/
│
├── main.py (or tic_tac_toe.py)       # Entry point – initializes game & GUI / logic  
├── game_logic.py                     # (Optional) Contains core logic: board state, move validation, win/draw check  
├── gui/                              # (Optional) GUI-related modules  
│   ├── ui.py                         # GUI layout, buttons/cells mapping to board  
│   ├── styles.py                     # (Optional) GUI styling / theme settings  
│   └── assets/                       # (Optional) Images/icons if used  
├── README.md                         # Documentation (this file)  
└── requirements.txt (optional)       # If external dependencies or for packaging  
```

**Details of each part:**

* `main.py` / `tic_tac_toe.py`: Entry script — sets up GUI or console version, loops through turns.
* `game_logic.py`: (If separated) Handles board representation (e.g. 2D list / array), validates moves, checks win/draw.
* `gui/`: Contains user interface code (buttons, event handlers, display), keeps GUI separate from logic (Model-View separation).
* `styles.py` / `assets/`: If using custom styling or images (icons for X/O, backgrounds).
* `requirements.txt`: If you use external modules (rare for simple game), else optional.

---

## 🐛 Troubleshooting & Tips

<details>
<summary>Click to expand possible issues</summary>

* **Game does not start / GUI window fails** — make sure Tkinter is installed and working.
* **Invalid move allowed / Overwriting cells** — ensure move validation logic checks for empty cell.
* **Win/draw detection fails** — ensure all eight win conditions (3 rows, 3 columns, 2 diagonals) are correctly coded. ([GeeksforGeeks][1])
* **No option to restart** — implement a reset method to clear board and restart state (player turns, board grid).

</details>

---

