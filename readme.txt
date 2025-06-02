# Space Shooters With GUI

A classic 2D space shooter game implemented in C++ using the [SFML](Simple and Fast Multimedia Library). This game features a graphical interface, player and enemy movement, shooting mechanics, scoring, and more.

## Features

- Player-controlled spaceship with keyboard input
- Enemy waves with increasing difficulty
- Score tracking and win/lose conditions
- Graphical user interface using SFML

## Prerequisites

### SFML Library

You must have SFML installed on your machine to compile and run the project.

- **Linux/macOS:** You can install SFML using your package manager or from source.
- **Windows:** Download the SFML SDK and set up your development environment accordingly.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/AyaanKhan1576/Space-Shooters-With-GUI.git
cd Space-Shooters-With-GUI
```

### 2. Compiling and Running

#### **On Linux/macOS**

Make sure you have SFML installed.  
For Ubuntu/Debian:

```bash
sudo apt-get install libsfml-dev
```

**Compile and run:**

```bash
# Compile the source file
g++ -c main.cpp

# Link and build the executable
g++ main.o -o sfml-app -lsfml-graphics -lsfml-window -lsfml-system

# Run the game
./sfml-app
```

#### **On Windows (using MinGW)**

1. Download and extract [SFML 2.5.1 for GCC MinGW]
2. Set the `SFML` folder path (e.g., `C:\SFML-2.5.1`).

**Compile and run:**

```bash
# Compile the source file (adjust the include path if needed)
g++ -IC:\SFML-2.5.1\include -c main.cpp 

# Link and build the executable (adjust the library path if needed)
g++ -LC:\SFML-2.5.1\lib .\main.o -o app.exe -lmingw32 -lsfml-graphics -lsfml-window -lsfml-system -lsfml-main -mwindows

# Run the game
./app.exe
```

**Note:**  
- Make sure `sfml-graphics`, `sfml-window`, `sfml-system`, and `sfml-main` libraries are in your SFML `lib` directory.
- Copy the `.dll` files from `C:\SFML-2.5.1\bin` to your executable's folder if you encounter missing DLL errors.

