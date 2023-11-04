# C-Project
This code is an implementation of a simple Snake and Ladder (also known as Chutes and Ladders) game in C. In this game, two players take turns rolling a six-sided die and moving their tokens along a game board. The game board contains squares numbered from 1 to 100, and certain squares are linked by ladders and snakes, which can either help or hinder the players' progress.

Here's an overview of the code's main components and how it works:

1. **Header Includes:**
   - The code includes three standard C libraries: `stdio.h` for input and output, `stdlib.h` for random number generation, and `time.h` to seed the random number generator.

2. **Function Definitions:**
   - `rollDie()`: This function simulates rolling a six-sided die and returns a random number between 1 and 6.
   - `printBoard()`: This function is responsible for printing the game board. It uses a 1D array to represent the board and alternates between printing from left to right and right to left to create the visual representation of the game board.
   - `movePlayer()`: This function takes the current player's position and the number rolled on the die as input. It calculates the new position of the player, accounting for ladders and snakes on the board.

3. **Global Variables:**
   - `player1` and `player2` store the positions of the two players on the game board.

4. **`main()` Function:**
   - The main function initializes the random number generator with a seed based on the current time.
   - It prompts the players to enter their names.
   - It enters a game loop that continues until one of the players reaches square 100 and wins.
   - Within the game loop, the players take turns rolling the die, moving their tokens, and updating their positions on the board.
   - The positions of snakes and ladders are defined in the `snakesAndLadders` array.
   - The game checks if a player lands on a snake, and if so, it displays a message.
   - The `printBoard()` function is called to display the updated game board after each player's turn.
   - When a player reaches square 100, the game declares that player as the winner and exits the loop.

Overall, this code implements a basic text-based version of the Snake and Ladder game for two players. The game uses random dice rolls and incorporates snakes and ladders as specified in the `snakesAndLadders` array to create an element of chance and excitement.
