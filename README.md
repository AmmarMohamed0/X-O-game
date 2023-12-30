# X-O Game

This Python code implements a simple X-O (Tic-Tac-Toe) game with a console interface. The game consists of several classes to manage the players, game board, and overall game flow.

## Code Explanation

### Player Class

- The `Player` class is responsible for storing player information such as name and chosen symbol.
- The `choose_name` method allows players to input their names, accepting only letters.
- The `choose_symbol` method prompts players to select a single letter as their game symbol.

### Menu Class

- The `Menu` class handles the display of menus, including the main menu and endgame menu.
- The `display_main_menu` method presents options to start or quit the game.
- The `display_endgame_menu` method displays options to restart or quit the game after it concludes.

### Board Class

- The `Board` class represents the game board, initialized with numbers from 1 to 9 to represent cell positions.
- The `display_board` method prints the current state of the board to the console.
- The `update_board` method allows players to make moves on the board.
- The `is_valid_move` method checks if a chosen cell is available for a move.
- The `reset_board` method resets the board to its initial state.

### Game Class

- The `Game` class manages the overall game, including players, the board, and game flow.
- The `start_game` method initiates the game based on the player's menu choice.
- The `setup_players` method collects player details, such as name and symbol.
- The `play_game` method controls the main game loop, allowing players to take turns until a win or draw occurs.
- The `check_draw` and `check_win` methods determine if the game is a draw or if a player has won.
- The `play_turn` method handles a player's turn, including input validation.
- The `switch_player` method alternates between players.
- The `quit_game` method prints a thank-you message when the player decides to quit.

### Usage

- The game is initiated by creating an instance of the `Game` class and calling the `start_game` method.

```python
game = Game()
game.start_game()
