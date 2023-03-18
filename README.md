## Game of Pig

This is a web-based implementation of the game of Pig using JavaScript. The game is played between two players with a single six-sided die. Each turn, a player repeatedly rolls the die until either a 1 is rolled or the player decides to "hold" and add the current total to their score. The first player to reach 100 points wins.

## How to Play

Load the index.html file in a web browser.

Click the "New game" button to start a new game.

Player 1 starts by clicking the "Roll dice" button.

After each roll, the dice value is added to the player's current score.

If the player rolls a 1, their turn ends and they score no points for that turn.

If the player clicks the "Hold" button, their current score is added to their total score and the turn ends.

Play alternates between the two players until one player reaches 100 points or more.

## Implementation Details

The game was implemented using JavaScript and HTML/CSS. The game board and dice are displayed using HTML and CSS, and the game logic is implemented using JavaScript.

The JavaScript code is organized into three sections:

1. Variable declarations: Here, the necessary variables are declared, including the player scores, the active player, the current score, and a variable to indicate whether the game is currently being played.

2. Function definitions: Two functions are defined here - switchPlayer() and init(). The switchPlayer() function is called whenever a player rolls a 1 or decides to hold. It updates the current score, switches the active player, and updates the UI to reflect the change. The init() function is called whenever a new game is started, and resets the game state to its initial values.

3. Event listeners: Three event listeners are set up to handle button clicks - one for rolling the dice, one for holding, and one for starting a new game. When the roll button is clicked, the rollDice() function is called, which generates a random dice value, updates the UI to show the new value, and updates the current score. If the dice value is 1, switchPlayer() is called. If the hold button is clicked, switchPlayer() is called if the active player's score is less than 100, otherwise the game is over and the winner is declared. Finally, when the new game button is clicked, the init() function is called to reset the game state.

## Logic

![logic](https://user-images.githubusercontent.com/58926340/226076938-d6c84095-8e35-4bf1-a78a-55fa7b13aa74.png)

## Screenshot

<img width="1440" alt="Screen Shot 2023-03-17 at 6 49 48 PM" src="https://user-images.githubusercontent.com/58926340/226076987-65289470-a459-467d-8c49-844054c54b3a.png">

