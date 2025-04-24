# 🎮 The 9 Tile Shuffle Game - Turbo C++ 

The 9-Tile Shuffle Game is inspired by classic sliding tile puzzles, offering a simple yet engaging experience that tests players’ problem-solving skills. 
The game consists of 8 numbered tiles and one empty space within a 3x3 grid. Players can slide adjacent tiles into the empty space to reorganize the grid. 
This project serves as an excellent practice for learning and applying C++ concepts such as arrays, loops, conditionals, and user input handling.


---

## 📝 Objectives:

1. Develop an interactive and visually clear sliding tile game using C++.
2. Provide an intuitive interface for players to move tiles.
3. Incorporate logic to verify the completion of the puzzle.
4. Enhance problem-solving skills by implementing efficient algorithms to manage tile movements and validations.

## 🎯 Game Aim:

Arrange the shuffled tiles named from **1 to 8** in ascending order on a **3x3 matrix board**, leaving one tile at the end blank.

```
Initial (Shuffled):        Final (Goal):
+---+---+---+               +---+---+---+
| 4 | 2 | 6 |               | 1 | 2 | 3 |
+---+---+---+               +---+---+---+
|   | 8 | 1 |     --->      | 4 | 5 | 6 |
+---+---+---+               +---+---+---+
| 3 | 6 | 7 |               | 7 | 8 |   |
+---+---+---+               +---+---+---+
```

---

## 📂 File Structure

```
/ShuffleGame
│
├── shufflegame.CPP     # Main Turbo C++ Source Code
└── README.md           # Project documentation
```

---

## 🧰 Technologies Used

- **Turbo C++ Graphics**
- `<graphics.h>`, `<conio.h>`, `<stdio.h>`, `<stdlib.h>`, `<string.h>`
- Classic DOS interface

## ⚙️ Algorithms Used:

-  Randomization algorithm to shuffle tiles while ensuring solvability.
-  Logic for detecting valid moves and updating the grid state.
-  Data Structure: The 3x3 grid is represented as a 2D array.
-  User Input: Players interact with the game using keyboard inputs to move tiles.
---

## 🕹️ How to Play

1. Use Turbo C++ (TC3) to compile and run the program.
2. When prompted:
   - Press `1` to start the game.
   - Press `2` to read the rules.
3. Use **keyboard number keys (1–8)** to move the specific numbered tile.
4. Keep sliding until all numbers are in ascending order until you reach the limit of 50 steps.
5. Press **X** anytime to exit the game.

---

## 📝 Features

- Intro animation with credits
- Menu interface with instructions
- Movement counter
- Valid move checker (prevents invalid moves)
- Victory screen with congratulations
- Max moves limit (50) for challenge
- Allows the player to restart the game with a new puzzle

---

## ⚙️ Compilation & Run (Turbo C++ only)

### 📦 Requirements

- Turbo C++ IDE (DOS-based)
- DOSBox (for modern systems)

### ▶️ Steps

1. Open **Turbo C++**
2. Load `shufflegame.CPP` locally in bin
3. Compile: `Alt + F9`
4. Run: `Ctrl + F9`

Ensure the BGI folder path is set correctly:
```cpp
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
```

---

## 🧠 Game Logic

- `initial()` – Initializes numbers randomly
- `check()` – Validates if a move is allowed
- `userwin()` – Checks if the player has arranged all tiles correctly
- `easy()` – Main game loop with drawing, input, and step counter
- `draw()` – Displays individual number tiles using ASCII box format

---

## 🎯 Winning Condition

The game is won when the `num[]` array contains numbers in this sequence:

```
[1, 2, 3, 4, 5, 6, 7, 8, 0]
```

Where `0` represents the blank tile.

---

## 🧱 Limitations

- **Turbo C++ specific**: Requires DOSBox or legacy environment.
- No support for mouse input or modern graphics.
- Limited to static shuffle pattern, not fully randomized.

---

## 💡 Future Improvements

- Port to modern C++ with SDL or SFML
- Add randomized puzzle generator
- Add score leaderboard
- GUI version with mouse/touch support

---

## 👤 Credits

Developed by: **Mansi Kumari**  
Language: **Turbo C++**  
Project Type: **Mini Project / Console Puzzle Game**

---

## 📜 License

Free to use, modify, and learn from!  
Distributed under the **MIT License**


