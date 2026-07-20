# STM32_Roboclaw
A lightweight STM32 wrapper for the official RoboClaw C++ library. It provides a C-compatible interface, allowing the original .cpp RoboClaw library to be used directly in STM32CubeIDE C projects without modifying the official source. Supports seamless UART communication with RoboClaw motor controllers.



# STM32 RoboClaw C Wrapper

This repository provides a C wrapper for the official RoboClaw C++ library, enabling it to be used in STM32CubeIDE C projects.

Since STM32CubeMX generates .c files while the RoboClaw library is written in C++, this wrapper bridges the gap by exposing C-compatible functions that internally call the original C++ implementation.

# Features
Compatible with STM32CubeIDE
Uses the official RoboClaw C++ library
C-compatible wrapper for .c projects
UART communication with RoboClaw motor controllers
No modifications required to the original RoboClaw library

# How It Works
1. Add the official RoboClaw C++ library to your STM32 project.
2. Include the wrapper header in your C source files.
3. Call the wrapper functions as you would any normal C library.
4. The wrapper internally invokes the corresponding C++ RoboClaw functions.

# Requirements
STM32CubeIDE
STM32 MCU
UART configured for RoboClaw communication
Official RoboClaw library
