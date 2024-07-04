# What is Artificial Intelligence?
In very simple terms, artificial intelligence is when you enable the computer to think like how a human would: predicting the weather for the next day, recognizing animals, considering which move to play next, are some examples of Artificial Intelligence.

# What is the Minimax Algorithm in Artificial Intelligence?
Minimax Algorithm is a type of search algorithm where the computer tries to find the best move to play in order for the computer to win. We assign a score to the possible moves in the game and evaluate the best possible move that maximizes the computer’s chance to win. One player (Player X) is assigned to be the “Max player” who try to maximize his score and the other player (Player O) is the “Min player”, minimizing his score. Going in-depth through every possibility and finding the best move for the computer to play in its favour is called the Minimax Algorithm.

# Understanding the Minimax Algorithm.
Consider the graph diagram below:
![image](https://github.com/Spooke02/Tic_Tac_Toe_AI/assets/88731398/26c50e33-f411-4c5a-b012-a921b272a1b1)

Say that we have a state that looks like the topmost (root) board, and it is the computer’s turn (Player O). The computer will aim to minimize the score as much as possible.

1. There are 3 moves available for the computer: top-right, middle-left and bottom-left.

2. After playing each of these moves, the computer will evaluate the possible moves of the user (Player X). The algorithm will recurse for the temporary updated state.

3. If the board is at a terminal state (orangish box), then it will return a specific value: 1 if X wins; -1 if O wins; and 0 if it’s a tie.

4. When the algorithm is evaluating the user’s (Player X’s) play, then it will maximize score — best move the user can play. When the algorithm is evaluating the computer’s (Player O’s) play, then it will minimize the score.

In the above example, at the root level, the 3 possible moves determine the score of a particular action. Playing top-right would result a +1 in the worst case. Playing middle-left would result a -1 in the worst case. Playing bottom-left would result a 0 in the worst case.

Since the computer is trying to minimize its score, it will choose to play the middle-left cell since it is the best play. In this case, the computer will win the game in the worst case. This is the Minimax Algorithm.
