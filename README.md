# 🎮 Tic Tac Toe in Python

A simple terminal-based **Tic Tac Toe** game for two players, built using pure Python. Play in turns, check for wins and draws, and enjoy nostalgic gaming right in your console.


## 📋 Features

- 2-player mode (alternating X and O)
- Input validation and error handling
- Win detection (rows, columns, diagonals)
- Draw detection (when board is full)
- Clean console UI with formatted board


## 🧠 How It Works

- The board is a 3x3 grid.
- Players take turns to place their symbol (`X` or `O`).
- A player wins if they align 3 of their symbols in a row, column, or diagonal.
- The game ends in a draw if the board is full with no winner.


### Prerequisites

- Python 3.x

📄 Code Explanation
`print_board(board)`

Displays the current board in a readable format with row separators.

`check_win(board, player)`
Checks whether the given player (either "X" or "O") has won:

+ 3 in any row
+ 3 in any column
+ 3 in either diagonal

`is_full(board)`
Checks whether the board is full (no empty spaces). If true and there's no winner, it's a draw.

`tic_tac_toe()`
Main game loop:
+ Initializes an empty 3x3 board.
+ Alternates between players for each turn.
+ Handles input and validations.
+ Calls win/draw checks.
+ Displays results and ends the game.

`if __name__ == "__main__"`
Ensures the game starts only when the file is run directly (not imported).


```bash
python tic_tac_toe.py
```

Output of the demonstration is displayed below

```py
PS D:\pycharm installed\procject\.venv\Scripts> python .\tic_tac_toe.py
Welcome to Tic Tac Toe!

  |   |
-----
  |   |
-----
  |   |
-----

Player X, enter row (0-2): 1
Player X, enter column (0-2): 2

  |   |
-----
  |   | X
-----
  |   |
-----

Player O, enter row (0-2): 0
Player O, enter column (0-2): 0

O |   |
-----
  |   | X
-----
  |   |
-----

Player X, enter row (0-2): 1
Player X, enter column (0-2): 3
Invalid move. Out of bounds!
Player X, enter row (0-2): 2
Player X, enter column (0-2): 4
Invalid move. Out of bounds!
Player X, enter row (0-2): 1
Player X, enter column (0-2): 2
That spot is already taken!
Player X, enter row (0-2): 0
Player X, enter column (0-2): 2

O |   | X
-----
  |   | X
-----
  |   |
-----

Player O, enter row (0-2): 2
Player O, enter column (0-2): 0

O |   | X
-----
  |   | X
-----
O |   |
-----

Player X, enter row (0-2): 2

O |   | X
-----
  |   | X
-----
O |   | X
-----

Player X wins!
```
