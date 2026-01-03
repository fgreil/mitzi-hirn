# mitzi-mens-magistra
A simple Flipper Zero combination cracking game.

<img alt="Mens Magistra Screen"  src="screenshots/MainScreen.png" width="40%" />

A one-player logic game where Flipper Zero creates a secret color code with 4 symols of 6 different colors . The user has to guess it in the fewest attempts. She/He receives clues: Black pegs for correct color/position, white pegs for correct color/wrong position.

## Usage
- **Left/Right**: Move Puck-girl through the maze
- **Up/Down**: Restart game (when game over or won)
- **OK**: Send guess for checking (only possible if all four digits have been populate).
- **Long OK**: Give up, i.e. reveal the combination
- **Back Button**: Pauses game or (when held) exits

## More info
The constant `COLOR_REPEAT` controls whether a color can repeat or not.  [default: FALSE]). When guessing, the user has to adjust the color of four 20px diameter circles. Colors are represented by different fill pattern. Empty, non-filled circles are reserved and mean that the user has not chosen a color yet.

On the top right we have the heads-up-display (HUD): 
* `T: [MMM:SS]` is timer
* `A: [number of attempts](12)`

The game continues until the player either correctly guesses the full sequence or runs out of attempts.

## Version history
See [changelog.md](changelog.md)

