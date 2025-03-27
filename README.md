
# Tetris Game - README 🎮

## Overview 🌟

This is a simple, console-based implementation of the classic *Tetris* game written in C++. The game includes the basic mechanics and user controls of Tetris, with some additional features such as wall-kick rotation and increasing game speed as you progress. The game is rendered in the console with colors representing different Tetrominoes, and it offers an engaging experience with real-time user input and dynamic gameplay. 🕹️

### Features ✨
- **Tetromino Shapes**: The game includes seven different Tetromino shapes:
  - **I-piece**: A long vertical or horizontal block. ➖
  - **O-piece**: A 2x2 square block. 
  - **T-piece**: A T-shaped block. 
  - **Z-piece**: A Z-shaped block. 
  - **S-piece**: An S-shaped block. 
  - **L-piece**: An L-shaped block. 
  - **J-piece**: A reverse L-shaped block. 

- **Rotation with Wall-Kick**: Tetrominoes can be rotated with wall-kick mechanics that allow for shifting left or right when a rotation is not possible. This helps prevent collisions with obstacles while rotating. 🔄

- **Game Speed**: The game starts at a moderate speed, but as the player clears lines and scores points, the speed gradually increases to provide a challenging experience. ⚡

- **Gravity and Soft/Hard Drop**: Tetrominoes fall automatically with gravity, and the player can speed up their descent using the Down arrow key (soft drop) or instantly drop the piece with the Spacebar (hard drop). ⬇️

- **Line Clearing**: When a row is filled completely, it is cleared, and the player earns points. The score increases with each line cleared, and the game adjusts its speed after every 500 points. 🧹

- **Game Over**: The game ends when a new Tetromino spawns and collides with existing blocks at the top of the screen. 🚫

### Controls 🎮
- **Arrow Keys**:
  - **Left Arrow**: Move the current Tetromino left. ⬅️
  - **Right Arrow**: Move the current Tetromino right. ➡️
  - **Up Arrow**: Rotate the current Tetromino. 🔄
  - **Down Arrow**: Soft drop the current Tetromino. ⬇️
  
- **Spacebar**: Hard drop the current Tetromino to the bottom. 🚀

- **Esc**: Exit the game. 🛑

### Console Colors 🎨
The game uses different colors for different Tetrominoes, making it easier to distinguish between them. Each Tetromino has its unique color, enhancing the visual appeal of the game. 🌈

### Game Mechanics ⚙️
- **Spawning Tetrominoes**: The game begins with a random Tetromino spawning at the top of the grid. The new piece spawns in the center of the grid horizontally. 🏁
  
- **Collision Detection**: The game constantly checks for collisions between the current Tetromino and the grid or other blocks. If a collision occurs, the piece stops, and a new Tetromino spawns. If the piece reaches the top of the screen, the game ends. 💥

- **Line Clearing**: When a full line is detected (i.e., no empty spaces in that row), the line is cleared, and all rows above it move down one row. This process rewards the player with points. 🎯

- **Increasing Speed**: As you accumulate points, the speed of the game increases, making it more challenging to place and rotate Tetrominoes. ⚡

### Scoring 🏅
- **100 points** for clearing a single line. 🏆
- **500 points** trigger a speed increase, making the game progressively harder. 🚀
- The final score is displayed when the game ends, providing a measure of the player's performance. 📊

### System Requirements 💻
- **Operating System**: Windows (due to the usage of `windows.h` for console color setting). 🖥️
- **C++ Compiler**: Compatible with any C++11 or later compiler. ⚙️
- **Libraries**:
  - `windows.h` for console manipulation (coloring). 🌈
  - `conio.h` for handling user input in real-time. ⌨️
  - `ctime` for random number generation based on time. ⏰

### How to Compile and Run 🚀
1. **Clone or Download the Source Code**:
   Download the `tetris.cpp` file to your computer. 📥

2. **Compile the Program**:
   Use any C++ compiler that supports the required libraries (e.g., GCC for Windows). If using GCC, you can compile the code with the following command:

   ```bash
   g++ -o tetris tetris.cpp
   ```

3. **Run the Program**:
   After compiling, run the executable:
   
   ```bash
   ./tetris
   ```

   Or, on Windows:

   ```bash
   tetris.exe
   ```

4. **Start Playing**:
   Once the game is running, use the arrow keys to control the Tetrominoes and enjoy the game! 🕹️



---

Enjoy playing Tetris! 🎮🎉
