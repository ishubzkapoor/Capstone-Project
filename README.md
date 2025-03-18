# CPPND: Capstone Snake Game Example

This is a starter repo for the Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). The code for this repo was inspired by [this](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) excellent StackOverflow post and set of responses.

<img src="snake_game.gif"/>

The Capstone Project gives you a chance to integrate what you've learned throughout this program. This project will become an important part of your portfolio to share with current and future colleagues and employers.

In this project, you can build your own C++ application or extend this Snake game, following the principles you have learned throughout this Nanodegree Program. This project will demonstrate that you can independently create applications using a wide range of C++ features.

## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  >Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source. 
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.


## CC Attribution-ShareAlike 4.0 International


Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

My Additions
Rubric points

README
## Loops, Functions, I/O
The project demonstrates an understanding of C++ functions and control structures : see "Controller.cpp", "Game.cpp" or "Snake.cpp".
The project accepts user input and processes the input : see "Controller.cpp" method "HandleInput" & "HandleInputPlayer2".
## Object Oriented Programming
The project uses Object Oriented Programming techniques : Snake Class, Game Class and Controller Class and their comunications.
Classes use appropriate access specifiers for class member : all members & functions are using the appropriate specifiers.
Class constructors utilize member initialization lists : Snake constructor in "Snake.h" for example.
Classes encapsulate behavior : all methods for a snake object are in Snake class for example.
## Memory Management
The project makes use of references in function declarations : see "Game.h" Line 14 (Run method) & "Controller.h" Line 8&9.
The project uses destructors appropriately.


## Concurrency
The project uses multithreading : see "Game.cpp" Line 29&30 (Run method)
the game now has 2 players that work togather to reach the highest score, the rules are:

--> the score is incremented if either of the players got ate a food (1 food = 1 point)
--> if a snake collides with another they both die.---
--> if a snake collides with its body it dies.
---> if either of the snakes dies the game is over.

