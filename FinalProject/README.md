## Final Project: Rock, Paper, Scissors Game
**Description:** Create a menu-driven rock, paper, scissors game in C# that a user plays against the computer with the ability to save and load a game and its associated play statistics. The game will also be able to display a leader board and global statistics.

**Project Files:** player_log.csv Download player_log.csv

**Requirements:** Create Rock.

Create a Rock, Paper, Scissors game C# project named finalProject according to the requirements specified in this document. The user plays against the computer with the ability to save and load a game and its associated play statistics. The game will also be able to display a leader board and global statistics for all players.

During a round of play the user chooses rock, paper, or scissors from a menu and the computer makes its choice randomly. For each round it is possible for the user to win, lose, or tie. The statistics that are to be maintained for a game are wins, losses, and ties. When a game is saved the user’s name and play statistics (wins, losses, and ties) are to be saved. When a game is loaded based on the user’s name the statistics are loaded and additional game play add to the loaded statistics.

### Rock Paper Scissors: Rules
- Rock beats scissors
- Scissors beats paper
- Paper beats rock


### Menus
For menus in the game, the user makes a selection from the menu by entering the number of their choice. If the user enters something other than a number or a number in the range of the choices provided in the menu they are to be given feedback that their choice is not valid and asked for the input again. Under no circumstance should input from the user crash the program.

When the program is run the following title, menu, and input prompt are to be displayed.
```
    Welcome to Rock, Paper, Scissors!

        1. Start New Game
        2. Load Game
        3. Quit

    Enter choice:
```

User Choices:

- 1. Starts a new game and the user is prompted for their name and game play is to proceed after their name is entered. There cannot be duplicate player names. If the player submits a name that already exists then they should be prompted to provide another name.
- 2. Loads a game and they should be taken to a prompt to enter a name that is to be used to load a saved game.
- 3. Quits the game and the program is to exit.


### 1. Start New Game

If the user chooses to start a new game the program is to prompt the user for their name using the following prompt.

    What is your name?
After the name is entered the program is to respond with a line that is “Hello” followed by the name of the user, a period, and the phrase “Let’s play!” Example:

    Hello Kristofferson. Let’s play!
After the hello statement is presented to the user, game play is to proceed. Game play is described below in the Game Play section.

### 2. Load Game


If the user chooses to load an existing game the program is to prompt the user for their name using the following prompt.

    What is your name?
After the name is entered the program is to attempt determine if saved game data for that player exists by searching through the saved game data loaded from the player log file you were given. If the player exists, the information about the game and statistics are to be loaded, a welcome back message is to be presented to the user, and game play is to proceed. The round number displayed is to be based on the number of rounds previously played. (Note: number of rounds previously played is sum of wins, losses, and ties.) Game play is described below in the Game Play section.

The welcome back message is to be “Welcome back” followed by the user’s name, a period, and the phrase “Let’s Play!” Example:

    Welcome back Kristofferson. Let’s play!
If the player is not found, the user is to be presented with a message indicating the game could not be found and then presented with the startup menu described at the top of the requirements. The message is to be the user name followed by “, your game could not be found.” Example:

    Kristofferson, your game could not be found.
 
 
### 3. Quit

If the user chooses to quit, the program is to exit.

### Game Play

This section describes game play.

For each round a line that includes the round number is to be displayed followed by a menu that let’s the user choose Rock, Paper, or Scissors as their choice for the round as shown below.

    Round <round number>

        1. Rock
        2. Paper
        3. Scissors

    What will it be?
The user makes their choice and the computer chooses randomly. The result of the round is to be displayed using the following format:

    You chose <user choice>. The computer chose <computer choice>. You <win/lose>!
Example:

    You chose Paper. The computer chose Rock. You win!
After the round the user is to be presented with the following prompt and menu.

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice:
If the user chooses 1 to play again, the user is to play another round. If the user chooses 2 to view player statistics, the current statistics for the game are to be displayed. If the user chooses 3 the leaderboard and several global stats are to be displayed. If the user chooses 4 to quit, the game and associated statistics are to be saved to the player log and the program is to exit.

### 1. Play Again

If the user chooses to play again the next round number is to be displayed and the user is to again choose Rock, Paper, or Scissors to play the round as described above.

### 2. View Statistics

If the user chooses to view the statistics the following information is to be displayed:

    <user name>, here are your game play statistics…
    Wins: <number of wins>
    Losses: <number of losses>
    Ties: <number of ties>

    Win/Loss Ratio: <wins divided by losses formatted to two digits
    to right of decimal point>

Example:

    Kristofferson, here are your game play statistics…
    Wins: 8
    Losses: 7
    Ties: 2

    Win/Loss Ratio: 1.14
After the statistics are displayed, the user is to be presented with the menu shown above that is presented after playing a round.

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice:
### 3. View Leaderboard

If the user chooses to view the leadrboard the following information is to be displayed (Top 10 players with wins, Top 5 players wo played the most games, Overall win/loss ratio, Total games played for (the sum of total games each player has played)):

    Top 10 Winning Players
    <player name>: <wins>
    <player name>: <wins>
    <player name>: <wins>
    <player name>: <wins>
    <player name>: <wins>
    <player name>: <wins>
    <player name>: <wins>
    ...
    
    Most Games Played:
    <player name>: <total games played>
    <player name>: <total games playe>
    <player name>: <total games playe>
    <player name>: <total games playe>
    <player name>: <total games playe>
    

    Overall Win/Loss Ratio: <total wins divided by losses formatted to two digits to right of decimal point>

    Total Games Played: <the sum of total games each player has played>

Example:

    Global Game Statistics
    ----------------------
    ----------------------
    Top 10 Winning Players
    ----------------------
    Bart: 9 wins
    Brad: 9 wins
    Daria: 9 wins
    Mina: 9 wins
    Ron: 9 wins
    Tania: 9 wins 
    Janae: 8 wins
    Enoch: 7 wins
    Rosalee: 7 wins
    Shay: 7 wins

    ----------------------
    Most Games Played
    ----------------------
    Brad: 24 games played
    Janae: 22 games played
    Rosalee: 20 games played
    Daria: 19 games played
    Enoch: 19 games played

    ----------------------
    Win/Loss Ratio: 1.49
    ----------------------

    ----------------------
    Total Games Played: 286
    ----------------------

### 4. Quit

If the user chooses to quit the game, the program is to automatically save the game and associated statistics in the player_log.csv file. If there is an exception saving the file, an error message reporting the error is to be presented to the user. The message is to be “Sorry ” followed by the user’s name and “, the game could not be saved.” Additionally, the actual error provided by the Exception object is to be displayed on the next line. Example:

    Sorry Kristofferson, the game could not be saved.
If the file saves successfully the user is to be presented with a message indicating the success of the file save. The message is to be the user’s name followed by “, your game has been saved.” Example:

    Kristofferson, your game has been saved.
Finally, the program is to exit.

### Player Log File Format

The data in the player_log.csv file is structured in the following way:

```
<player name>, <wins>, <losses>, <ties>
```

Data must be saved in that format.

Coding Style: You are encouraged to develop your application in a modular style, by creating functions to perform the major functionality of the application. This will make your code much easier to develop, maintain, and debug. You should determine an appropriate data format for you player data. Consider creating a Struct or a Class to store playes data.

## Sample Game Output

### Example 1
    Welcome to Rock, Paper, Scissors!

        1. Start New Game
        2. Load Game
        3. Quit

    Enter choice: 1

    What is your name? 

    Hello Kristofferson. Let’s play!

    Round 1

        1. Rock
        2. Paper
        3. Scissors

    What will it be? 2

    You chose Paper. The computer chose Rock. You win!

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice: 1

    Round 2

        1. Rock
        2. Paper
        3. Scissors

    What will it be? 1

    You chose Rock. The computer chose Paper. You lose!

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice: 2

    Kristofferson, here are your game play statistics…
    Wins: 1
    Losses: 1
    Ties: 0
    Win/Loss Ratio: 1.00

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice: 4

    Kristofferson, your game has been saved.

### Example 2
    Welcome to Rock, Paper, Scissors!

        1. Start New Game
        2. Load Game
        3. Quit

    Enter choice: 2

    What is your name? Kristofferson

    Welcome back Kristofferson. Let’s play!

    Round 3 // Note: this is round 3 because two other rounds were in a saved file!

        1. Rock
        2. Paper
        3. Scissors

    What will it be? 3

    You chose Scissors. The computer chose Paper. You win!

    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit
    
    Enter choice: 3

    Global Game Statistics
    ----------------------
    ----------------------
    Top 10 Winning Players
    ----------------------
    Bart: 9 wins
    Brad: 9 wins
    Daria: 9 wins
    Mina: 9 wins
    Ron: 9 wins
    Tania: 9 wins 
    Janae: 8 wins
    Enoch: 7 wins
    Rosalee: 7 wins
    Shay: 7 wins

    ----------------------
    Most Games Played
    ----------------------
    Brad: 24 games played
    Janae: 22 games played
    Rosalee: 20 games played
    Daria: 19 games played
    Enoch: 19 games played

    ----------------------
    Overall Win/Loss Ratio: 1.49
    ----------------------

    ----------------------
    Total Games Played: 286
    ----------------------
    
    What would you like to do?

        1. Play Again
        2. View Player Statistics
        3. View Leaderboard
        4. Quit

    Enter choice: 4

    Kristofferson, your game has been saved.
