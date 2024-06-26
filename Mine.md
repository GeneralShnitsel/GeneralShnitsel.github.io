---
layout: default
---

[<button>Home</button>](./)
&nbsp;&nbsp;[<button>Portfolio</button>](./portfolio.html)
&nbsp;&nbsp;[<button>Contact</button>](./Contacts.html)&nbsp;&nbsp;


## This is Minesweeper but in First person and 3D

I recreated the game of MineSweeper but put a twist on it and created the gameboard as a walkable platform that the player can traverse across with a first person character and uncover the tiles on the ground one by one to solve the puzzle of minesweeper and beat the game from an alternative perspective compared to the original 2D grid that the original game operates in.

<img src="Images/CleanBoard.PNG" alt="Clean board">

This is done by first assigning each block with a bomb or a number based on a predetermined chance (20% chance) which is how the gameboard is populated with bombs. Once the board has been populated I use a script that detects how many bombs are around it to then assign said square a number corresponding to the amount of bombs sorounding the specific tile.

<img src="Images/Failed Board.PNG" alt="Failed board">

The player navigates across the board with the First Person Character uncovering tile after tile slowly solving the puzzle. 

<img src="Images/Placer.PNG" alt="Placer">

MinePlacer is the script responsible for determining which tiles will or will not have a bomb in them by assigning each tile a chance to be a bomb at the start of the game and then populting the entire board with momb tiles and number tiles. The script also looks for other Mine Detectors nearby which is a component on each tile that displays a number corresponding to the amount of bombs around it and this data

<img src="Images/Detector1.PNG" alt="Detector1">
<img src="Images/Detector2.PNG" alt="Detector2">

This script attaches sprites to the tops of the tiles depending on the mine count that has been calculated by the Mine detectors that were populated to each tile at the start of the game. I have done this by running a check on each mine detector to get the mine count value so that the correct number sprites are labeled on each of the respectful tiles. If the player hits a bomb tile the tile turns red and the player loses the game to then restart or continue playing.