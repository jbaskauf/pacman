# JavaFX GUI Implementation of Pac-Man
This JavaFX Pac-Man implementation is a class project from CS257 Software Design (taught by Jeff Ondich at Carleton College), completed collaboratively with Ellie Mamantov. It uses the Model-View-Controller pattern to create a well-structured application that keeps track of game state, displays current game state, and reacts to user input.

![Level 1](level1screen.png)

## Features
Implements most typical features of Pac-Man. The user can press the arrow keys to dictate the direction that Pac-Man is moving, and he is chased by two ghosts that move randomly unless they are in the same row or column as Pac-Man, in which case they move towards him in the normal mode, or move away from him if he has recently eaten a big dot. Changes in the Model are driven by key and timer events. Current score, level, and Game Over/You Won! messages are displayed in Labels at the top of the window, which are updated continuously to reflect changes in the Model.

Users can play three different levels and start new games by pressing G. Level map layouts are each stored in a text file that encodes the various screen components based on this system:
- "W" indicates a wall
- "E" indicates an empty square
- "B" indicates a big dot
- "S" indicates a small dot
- "1" and "2" indicate the ghosts' homes
- "P" indicates Pacman's starting position

Three levels are provided, but more could be added to the levels folder in the future using this system (level file names must also be added to the list of level filename strings in the Controller class).

## Repo structure
```
├── README.md                 : Description of this repository
├── improvements.txt          : Reflections on bugs and imperfections remaining at the end of the project, to be improved in the future
├── pacman.iml                : IntelliJ module file
├── src                       : Project code and resource files
│   ├── finalPacman           : MVC java files and fxml layout file
│   ├── levels                : Text files containing level layout information (interpreted by the Model when initialized)
│   └── res                   : Image files (png and gif)
└── .gitignore                : Files and directories to be ignored by git
```

### Contributors
Jessie Baskauf

Ellie Mamantov
