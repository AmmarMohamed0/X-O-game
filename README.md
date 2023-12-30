# X-O-game
"X-O Game: Python console-based Tic-Tac-Toe. Customize players, symbols, and enjoy interactive gameplay. Dynamic board, win/draw detection, and user-friendly menus. Clear screen for a polished interface. Compete, restart, or quit. A modern take on a timeless game."
#  Explanation of the provided Python code for an X-O game:
clear_screen Function:
Clears the terminal screen based on the operating system (Windows or other).
Player Class:
Represents a player in the game.
Attributes:
name: Player's name (initialized as an empty string).
symbol: Player's chosen symbol (initialized as an empty string).
Methods:
choose_name: Takes user input for the player's name, allowing only letters.
choose_symbol: Takes user input for the player's symbol, allowing only a single letter.
Menu Class:
Manages the game menus.
Methods:
display_main_menu: Displays the main menu with options to start or quit the game.
display_endgame_menu: Displays the endgame menu with options to restart or quit.
get_valid_input: Takes user input with a prompt and a list of valid options, repeating until a valid input is received.
Board Class:
Represents the game board.
Attributes:
board: List representing the game board with cell numbers initially.
Methods:
display_board: Prints the current state of the game board.
update_board: Updates the board with the player's move if the move is valid.
is_valid_move: Checks if a move is valid by verifying if the chosen cell is a digit.
reset_board: Resets the game board to its initial state.
Game Class:
Manages the overall game.
Attributes:
players: List containing two Player objects.
board: Board object representing the game board.
menu: Menu object for managing menus.
current_player_index: Index (0 or 1) of the current player.
Methods:
start_game: Initiates the game based on user menu choice.
setup_players: Takes player details (name and symbol) for both players.
play_game: Controls the flow of the game, including turns and endgame conditions.
restart_game: Resets the board and restarts the game.
check_draw: Checks if the game is a draw.
check_win: Checks if there is a winner based on win combinations.
play_turn: Manages a player's turn, taking input for cell choice.
switch_player: Switches the current player.
Game Execution:
Creates a Game object.
Calls start_game to begin the game execution.
