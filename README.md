# 2048Game
2048 Game with Pygame
Overview
This is a Python implementation of the classic 2048 game using the Pygame library. The game allows players to slide tiles on a grid and merge tiles with the same numbers. The goal is to reach the 2048 tile. The game features a graphical interface with keyboard controls and includes additional elements such as a top toolbar, user ID input, score tracking, high score counter, and a reset button.

#Features
Graphical interface using Pygame.
Responsive layout that adjusts to window size changes.
User-friendly toolbar with essential controls:
Reset button to restart the game.
Display of user ID, current score, and high score.
Confirmation message when resetting the game to prevent accidental resets.
High score tracking stored in a text file.
#How to Run
Ensure you have Python installed on your system.
Install the Pygame library by running pip install pygame.
Download or clone this repository.
Run the 2048_game.py file using Python.
#Code Functions
initialize_fonts()
Initializes the fonts used in the game interface based on window dimensions.

resize_elements()
Adjusts the sizes of elements such as toolbar height and tile size based on window dimensions.

draw_tile(x, y, value)
Draws a single tile with the specified value at the given coordinates.

draw_grid(grid)
Draws the entire grid based on the current state of the game.

draw_toolbar(user_id, score, high_score)
Draws the top toolbar containing user ID, current score, high score, and reset button.

generate_tile(grid)
Generates a new tile with a value of either 2 or 4 at a random empty position on the grid.

move_tiles(grid, direction)
Moves tiles on the grid in the specified direction (up, down, left, or right) and merges tiles with the same values.

is_game_over(grid)
Checks if the game is over by verifying if no more moves are possible.

get_user_id()
Prompts the user to enter a unique user ID before starting the game.

save_score(user_id, score)
Saves the user's score to a text file along with their user ID.

load_high_score()
Loads the highest score recorded from the score file.

reset_scores()
Clears the score file to reset all recorded scores.

draw_confirmation_box()
Draws a confirmation message box when the reset button is pressed, allowing the user to confirm or cancel the reset action.

#Build Explanation
The game is built using the Pygame library, which provides a simple yet powerful framework for creating 2D games in Python. The main game loop handles user input, updates the game state, and renders the game graphics. Additional functions are implemented to manage game mechanics, display elements, and handle user interactions.

