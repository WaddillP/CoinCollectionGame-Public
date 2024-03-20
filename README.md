# CoinCollectionGame-Public

The character is a spaceship. There are 5 levels and on each level there are coins to collect as well as enemies to
avoid. The character is controlled by the arrow keys. The character has 3 lives, and you have 30 seconds to collect
every coin on each level. Lives do not reset between levels. If you run out of health or time you lose the game, if
all levels are completed you win the game. To run the game make sure the sprites are in the same folder as the game and
press the play button.

Basic Features:
User input: to move the character

Uses character.x += depending on what key is being pressed, the character can move faster than the enemies

Game Over: Once 3 enemies are hit and the health bar hits 0 the game ends

if the health variable hits 0 game over screen will ensue

Graphics/Images: the character is a spaceship, the enemies are pacman enemies and the coins are well coins.

Additional Features:
Enemies: Multiple enemies will be moving towards the character trying to make it lose health. Enemies are held in a
dictionary of lists that correspond to each level that they occupy. Once all coins are collected the level variable
increases by one and the correct enemies list shows up. If an enemy makes contact with the character then the characters
health will decrease by 1 and the enemy will be spawned into one of the 4 corners randomly.

Collectibles: Coins also live in a dictionary of lists that correspond to each level. Once they are made contact with
they are moved off of the screen and an integer called score is increased. Once score equals the level then level
increases and score is reset to 0. Each level with have a number of coins that is equal to level (level 4? 4 coins).
Once all coins are collected it uses this to level up the game.

Health Bar: A health bar will be visible to indicate how many times an enemy can hit the user until they die. Will be
using a health function that will have an if statement using an integer variable called health that changes the image
representing how much health is left. A health function is used to do this that checks how much health is equal to then
updates the image accordingly.

Multiple Levels: Once all the coins are collected on a level a new level will be made and there will be more coins to
get and more enemies --> the levels will progressively get more and more difficult. Once a new level is reached the
level variable is incremented by 1 and the dictionaries change the amount of enemies and coins that are on the screen to
match what level the player is on.

Timer: There is a timer in the bottom left corner that indicates how much time you have until you lose per level. If you
run out of time, you lose. The timer resets each level. This uses a timer variable that is incremented every time tick
is called --> 30 times per second. Then there is a function that is made to update the countdown that will have an if
statement checking when timer is divisble evenly by 30 which will be once every second. It also updates the text based
on what the countdown variable is equal to, countdown is reset every level. If it hits 0 the game is over.

Teleporting: There are gaps in the walls in the middle of the 4 sides, each one teleports you to the opposite one. Left
Teleports to right, top teleports to bottom etc.

Code Utilizes UVAGE, a private University of Virginia Game Engine in Python, due to this Code is not available.
