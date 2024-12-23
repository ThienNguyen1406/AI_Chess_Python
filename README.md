# Building chess game using artificial intelligence

## I. Method content

Applicable methods:

- Alpha-Beta Prunning and Minimax algorithms
- Heuristic evaluation functions

### 1.

#### 1.1 Minimax algorithm

** Minimax ** is an algorithm as a recursive algorithm to choose the next step in a game with two people by comparing node on the game tree.

! [Alt Text] (Result/Pseudo_code_Minimax.png)

- ** Advantages: ** Searching for every country to follow and then choose the best water.
- ** Disadvantages: ** For games with large state space such as chess, only the application of the Minimax algorithm is no longer effective due to the great combination explosion.

#### 1.2 Alpha-Beta Prunning algorithms

** Alpha-Beta Prunning ** was born and gradually replaced the Minimax algorithm. One of the noticeable advantages is to streamline the process of finding, eliminating some inappropriate cases arising and still ensuring no effect on the end result.

! [Alt Text] (Result/pseudo_code_alphabeta.png)

### 2. Heuristic evaluation functions

Using 2 basic assessment functions are: ** The total score of each chess pieces ** and ** points according to the position of each army **

Because each chess piece will promote all the strengths based on its position on the chessboard. Therefore, each chess pieces will have a $ 8 × 8 reward matrix.

Flagpion points:
! [] (Result/Scores.png)

Score according to the position of good troops:
! [Alt Text] (Result/Pawn_scores.png)





## II. Running program

Request Python 3.8

`` ``
PIP Install -R Requirement.txt

python game.py
`` ``

## III. Result

---

1. The game has 2 modes:

- People with people
- People with the machine

! [IMG.PNG] (Result/Menu.png)

2. Support shortcuts:

- Key Z: Undo again
- R keys R: reset the game

And the features suggest possible water, history of traveling countries, ...

! [img.png] (Result/Gameplay.png)

## Reference

https://www.chessprogramming.org/main_page