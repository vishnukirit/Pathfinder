# Pathfinder
This Python project is a simple maze-solving algorithm that utilizes the `curses` library to visually navigate through a maze using **Breadth-First Search (BFS)**.

The maze consists of walls represented by `#`, an entry point represented by `O`, and an exit point represented by `X`. The algorithm attempts to find the shortest path from `O` to `X` and displays it on the terminal.

## Features
* **Visual Maze Navigation:** Uses the `curses` library to display the maze in the terminal.
* **Breadth-First Search (BFS):** Implements BFS to find the shortest path from the start to the exit.
* **Real-time Visualization:** The pathfinding is displayed in real-time, showing how the algorithm explores the maze.

## How it Works
1. The maze is defined as a 2D list, where `#` are walls, `" "` are open spaces, `O` is the start, and `X` is the goal.
2. The algorithm searches for the shortest path using BFS.
3. The maze is printed using the `curses` library, with colors to differentiate the path (`X`) and walls (`#`).
4. Each step of the algorithm is shown in the terminal with a delay, allowing you to see how it explores different paths.

## Technologies Used
* **Python:** Core programming language.
* **Curses Library:** For rendering the maze and pathfinding in the terminal.
* **Queue Module:** Used for implementing the BFS algorithm.

## Installation
1. Clone the repository to your local machine:
```markdown
```bash
git clone https://github.com/yourusername/Pathfinder.git
cd pathfinder
```
2. Install the necessary dependencies:
```markdown
```bash
pip install windows-curses
```
**Note: The `curses` library is not available on Windows by default, so you need to install `windows-curses`. On Linux/macOS, the `curses` library is included in the standard Python distribution.**

## Usage
1. Navigate to the directory where the script is located.
2. Run the script:
```markdown
```bash
python maze_solver.py
```
3. The maze will be displayed in your terminal, and the algorithm will start finding the path from `O` to `X`.

## Maze Configuration
The maze is hardcoded as a 2D list. You can modify the `maze` variable in the script to create different maze configurations. For example:
```markdown
```python
maze = [
    ["#", "O", "#", "#", "#", "#", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", " ", "#", "#", " ", "#", "#", " ", "#"],
    ["#", " ", "#", " ", " ", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", "#", "#", "#", "#", "#", "#", "X", "#"]
]
```
## Example Output
![Screenshot (573)](https://github.com/user-attachments/assets/db02c6e9-9f90-4cbb-b442-2f96a930fd5a)

In the visual output, the shortest path will be highlighted in red, showing the algorithm's progress as it reaches the goal.

## License
This project is open-source and available under the `MIT License`.
