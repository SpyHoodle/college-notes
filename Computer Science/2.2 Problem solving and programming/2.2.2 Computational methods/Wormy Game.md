# Abstraction & Decomposition in Wormy
2022-09-13 Tue | [[2.2.2 Computational methods]]
## Code
- Functions are used throughout the code to abstract certain modules after decomposition
- `import pygame` is game library that is abstracted as we don't need to know how it works and is completely separate from the main code
## Game
- The user doesn't need to know about how the worm moves, only how to move it
- The user knows how to get score without understanding the code of how it gives them the score

![[2022-09-13-decomposition-diagram-wormy-game.png]]