Overview

A terminal-based Snake game built completely from scratch in C++. This project focuses heavily on:
- Low-level memory management
- Pointer manipulation
- Linked lists
- Cross-platform keyboard input
- Real-time game loops
- Object-oriented programming in C++
Unlike the Python version, this implementation required manual memory management and custom OS-specific keyboard handling.


Features

- Real-time snake gameplay
- Manual linked-list snake implementation
- Dynamic snake growth
- Collision detection
- Cross-platform keyboard input:
  - Windows
  - Linux/macOS
- Real-time terminal rendering
- Manual frame timing
- Dynamic food spawning
- Score tracking


Technologies Used

- C++
- STL containers:
  - map
  - pair
  - vector
- System libraries:
  - termios
  - unistd
  - conio.h
- Multi-file project architecture


Key Technical Highlights

Manual Memory Management: The snake body uses dynamically allocated nodes:
link* next;
link* prev;
A custom destructor cleans up all allocated memory when the game exits.

Cross-Platform Keyboard Handling: Custom keyboard.hpp implementation:
- Windows support using conio.h
- Linux/macOS support using:
  - termios
  - select()
  - raw terminal mode

Rendering System: The board is rendered manually using a 2D charater array:
cha board[BOARDLENGTH][BOARDWIDTH];


Controls

The good old WASD.


Building and Running:

Linus/macOS:
g++ main.cpp -o snake
./snake

Windows: Compile using:
- MinGW
- Visual Studio
- g++
example:
g++ main.cpp -o snake.exe
snake.exe


Project Structure

terminal-snake-c++/
|
|-main.cpp
|-keyboard.hpp
|_README.md


What I learned

- Pointer manipulation
- Dynamic memory management
- Linked list implementation in C++
- Cross-platform terminal programming
- Real-time systems programming
- Game architecture design
- Terminal rendering optimization


Future Improvements

- Better rendering performance
- Difficulty levels
- Smarter rendering system
