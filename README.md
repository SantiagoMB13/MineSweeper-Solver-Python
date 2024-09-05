# MineSweeper-Solver-Python

This project implements an automated Minesweeper solver using computer vision and artificial intelligence techniques. It captures the game board from the screen, analyzes it, and suggests safe moves.

## Features

- Screen capture of the Minesweeper game board
- Image processing to detect and extract the game grid
- Optical Character Recognition (OCR) to read cell values
- AI algorithm to determine safe moves
- Visualization of the detected board and suggested moves

## Requirements

- Python 3.x
- OpenCV
- NumPy
- EasyOCR
- PyAutoGUI
- Matplotlib

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/SantiagoMB13/MineSweeper-Solver-Python.git
   ```

2. Install the required dependencies:
   ```
   pip install opencv-python numpy easyocr pyautogui matplotlib
   ```

## Usage

1. Open a Minesweeper game in your browser (e.g., https://www.solitar.io/buscaminas)
2. Ensure the game board is visible on the left half of your screen
3. Run the main script:
   ```
   python minesweeper_solver.py
   ```
4. The program will capture the screen, detect the game board, and suggest a safe move

## How it works

1. **Screen Capture**: The program captures the left half of the screen using PyAutoGUI.
2. **Grid Detection**: OpenCV is used to detect the Minesweeper grid in the captured image.
3. **Cell Recognition**: EasyOCR reads the numbers in each cell of the grid.
4. **Game State Analysis**: The program constructs a matrix representation of the game state.
5. **Safe Move Calculation**: An AI algorithm analyzes the game state to determine safe moves.
6. **Visualization**: Matplotlib is used to display the detected game board and highlight the suggested safe move.

## Contributors

- David Daniel Henriquez Leal
- Santiago Andres Mercado Barandica
