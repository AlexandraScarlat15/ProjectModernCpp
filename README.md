# Modern Multiplayer Game Lobby – C++ Qt Client

Una Nueva Galaxia is a multiplayer game inspired by Battle City, where players control rockets in dynamic arenas, join or host matches, and experience smooth gameplay through a modular client-server architecture. This is a **team-developed modular C++ desktop application** built with Qt, designed to manage multiplayer sessions, user settings, and real-time interaction with a game server. 


## Features

- User login and session management
- Create or join multiplayer game sessions (multi-gaming support)
- Display room code for easy sharing and joining
- Server-client architecture with real-time communication via `ClientServer` class
- Level and game mode selection with smooth navigation
- In-game and general settings windows (configurable controls, audio, etc.)
- Game over screen with restart or exit options
- Support for multiple users with individual key bindings
- SQLite database integration for storing:
    - Registered players
    - Key mappings (custom controls per player)
- Modular window-based design using Qt for a clean GUI experience


## Technologies Used

- **C++ (Modern OOP practices)**
- **Qt 6 Widgets** – for GUI components
- **CMake** – cross-platform build system
- **Visual Studio (.sln)** – Windows development environment

## Structure Overview

ProjectModernCpp-main:
  .gitignore: Git ignore rules
  CMakeLists.txt: CMake build configuration
  README.md: Project documentation

  Client:
    Client:
      - "*.cpp, *.h": GUI components (Login, GameOver, etc.)
      - "ClientServer.cpp, .h": Networking logic
      - "*.ui": Qt Designer UI files
      - "*.qrc": Qt resource files
      libs:
        - "json.hpp": JSON handling via nlohmann/json
      resources:
        - "*.png, *.jpg": Game images and UI assets
    Client.sln: Visual Studio solution

  ProjectModerenCpp:
    - "*.cpp, *.h": Game logic (Bomb, Bullet, GameManager, etc.)
    - "*.db": SQLite databases (test or saved state)
    - CMakeLists.txt
    - Main.cpp

## Video Demo link :
https://youtu.be/ethhUT_XoZE
