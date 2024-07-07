# AI_powered_2048
Implementing an AI for the 2048 game using expectimax search. Model the AI player as a max player and the computer as a chance player. Create a depth-3 game tree to compute decisions for the AI player. Use the game engine's score as the evaluation function at the leaf nodes. Improve your AI to reach 512 tiles and a score over 5000.

Here's a GitHub description for the "Assignment 2: 2048" project:

---

### Task To Complete

Model the AI player as a max player and the computer as a chance player (placing a random 2-tile). Implement a depth-3 game tree and the expectimax algorithm to make decisions for the AI player. The evaluation function at the leaf nodes of the depth-3 game tree should use the score returned by the game engine.

The depth-3 game tree levels:
- Root: player
- Level 1: computer
- Level 2: player
- Level 3: terminal with payoff

The tree represents player-computer-player sequences. Compute the expectimax values for all nodes and return the optimal move. The starter code currently returns a random move. Proper implementation should frequently reach 512 tiles and a score over 5000.

### Usage

To run the program:
```bash
python main.py
```

Test the AI with the depth-3 tree and expectimax algorithm:
```bash
python main.py -t 1
```

In-game keyboard options:
- `r`: restart the game
- `u`: undo a move
- `3`-`7`: change board size
- `g`: toggle grayscale
- `e`: switch to extra credit

### Extra Credit (3 points)

Improve performance by either searching more depth or enhancing the evaluation function. Implement a stronger AI in the `compute_decision_ec` function in `ai.py`. Press `e` to toggle decisions made by this function. Achieve a score of more than 20,000 on at least 4/10 runs to earn extra points.

To test your extra credit implementation:
```bash
python main.py -t 2
```

