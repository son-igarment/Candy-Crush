# Candy Crush Game by Phạm Lê Ngọc Sơn

A Candy Crush clone game developed using SDL2 in C++.

![Candy Crush Preview](candy%20preview.gif)

## Project Description

This is a clone of the popular Candy Crush mobile game, implemented as a desktop application. The game features colorful graphics, sound effects, animations, and classic match-3 gameplay. Players match candies in groups of three or more to score points and progress through levels.

## Features

- Match-3 gameplay mechanics
- Colorful candy graphics and animations
- Sound effects and background music
- Score tracking system
- Level progression
- Win/lose conditions
- Interactive menu system

## Project Structure

The project is organized as follows:

```
Candy-Crush/
├── Candy Crush/                   # Main project directory
│   ├── Candy Crush/               # Source code directory
│   │   ├── Game/                  # Game assets directory
│   │   │   ├── candy spritesheet.png  # Candy graphics
│   │   │   ├── candy.ttf          # Game font
│   │   │   ├── *.wav, *.ogg       # Sound effects and music
│   │   │   ├── *.jpg, *.png       # Background images and icons
│   │   │   ├── *.gif              # Game animations
│   │   │   └── level.txt          # Level data
│   │   ├── SDL2/                  # SDL2 core library
│   │   ├── SDL2_image/            # SDL2 image extension
│   │   ├── SDL2_mixer/            # SDL2 audio extension
│   │   ├── SDL2_ttf/              # SDL2 font extension
│   │   ├── Module*.cpp/h          # Game engine modules
│   │   ├── Candy*.cpp/h           # Candy game logic
│   │   ├── CEV_gif*.cpp/h         # GIF handling library
│   │   ├── Main.cpp               # Game entry point
│   │   ├── Application.cpp/h      # Main application class
│   │   └── Globals.h              # Global definitions
│   └── Candy Crush.sln            # Visual Studio solution file
├── LICENSE                        # MIT License
└── README.md                      # This file
```

### Core Components

- **Module System**: The game is built using a modular architecture with specialized components:
  - `ModuleWindow`: Handles window creation and management
  - `ModuleRender`: Handles rendering operations
  - `ModuleInput`: Manages user input
  - `ModuleAudio`: Handles sound effects and music
  - `ModuleSceneIntro`: Main menu and introduction screens
  - `ModuleSceneGame`: The actual gameplay implementation
  - `ModuleFadeToBlack`: Scene transition effects

- **Candy Game Logic**:
  - `Candy`: Base candy object
  - `CandyGrid`: The game board implementation
  - `CandyMatch`: Match detection logic
  - `CandyScore`: Score tracking system

## Requirements

- Windows operating system
- Visual Studio (2017 or newer recommended)
- SDL2 library (included in the project)

## How to Use

1. **Open the Project**:
   - Open "Candy Crush.sln" in Visual Studio

2. **Build the Project**:
   - Set the build configuration to "Debug" or "Release"
   - Build the solution (F7 or Ctrl+Shift+B)

3. **Run the Game**:
   - Press F5 or click the "Start" button in Visual Studio
   - Alternatively, run the compiled executable from the output directory

4. **Gameplay**:
   - Use the mouse to select and swap candies
   - Match 3 or more identical candies in a row or column to score points
   - Complete the level objectives to advance

## Credits

- Developed by: Phạm Lê Ngọc Sơn
- Graphics and Sound: Various resources adapted for the game
- Built with: SDL2 library and C++

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.