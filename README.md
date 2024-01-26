# chess-ai
A minimax based active information directed tree search model that plays chess, created for a University assignment.

Make an attempt at beating it and let me know how you did! ♟️

### How it works

Using a variant of [Monte-Carlo Tree Search](https://en.wikipedia.org/wiki/Monte_Carlo_tree_search#Monte_Carlo_tree_search_(MCTS)), the chess AI simulates the outcomes of a set of different move choices either until the game ends or until a set tree depth is reached. The path leading to the best resulting game state is strengthened using backpropagation. Since [chess pieces are valued differently](https://www.chess.com/terms/chess-piece-value#Chesspiecevals), and the AI evaluates multiple moves ahead, it will sacrifice a piece or bait you into a certain next move if it expects it to more probably lead to a better overall game state down the line. The decision heuristic follows the [minimax method](https://en.wikipedia.org/wiki/Minimax). In other words, it directs its knowledge search and makes decisions to minimize your possible gain, in the case of optimal play.

#### Gameplay demo
![gameplay-gif](./readme_assets/sc-superfast-169.gif)

### Installation

1. Clone the project
2. Install the necessary requirements using `pip install -r requirements.txt`. If `tk` fails (common on macOS), install it using brew: `brew install python-tk`.
3. Run the start script `play.py`
4. Play using the GUI!

#### How to play

You start as whites. Click on a piece and then click it's location. The game does support castling, and will prevent you from making any illegal moves.
