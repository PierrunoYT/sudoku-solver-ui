# Sudoku Solver with GUI

A fast Sudoku puzzle solver implementation with a graphical user interface built using Python and Tkinter.

## Features

- Fast solving algorithm using backtracking with constraint propagation
- User-friendly GUI interface
- Input validation
- Clear visualization of 3x3 boxes
- Comprehensive logging system
- Error handling for invalid inputs

## Requirements

- Python 3.x
- Tkinter (usually comes with Python)

## Installation

1. Clone this repository:
```bash
git clone <repository-url>
```

2. Navigate to the project directory:
```bash
cd sudoku-solver
```

## Usage

Run the application:
```bash
python sudoku_gui.py
```

### How to Use

1. Launch the application
2. Enter numbers (1-9) in the cells where you know the values
3. Leave empty cells where you want the solver to find values
4. Click "Solve" to find the solution
5. Click "Clear" to reset the board

### Logging

The application logs all operations to both:
- Console output
- A file named 'sudoku.log'

Log levels:
- INFO: General operations (solving attempts, solutions found)
- DEBUG: Detailed solving steps
- WARNING: Issues like unsolvable puzzles

## Project Structure

- `sudoku_gui.py`: Contains the GUI implementation using Tkinter
- `sudoku_solver.py`: Contains the solving algorithm and logic
- `sudoku.log`: Log file generated during runtime

## Algorithm

The solver uses a backtracking algorithm with constraint propagation:
1. Find an empty cell
2. Try numbers 1-9 in the cell
3. Check if the number is valid in the current position
4. If valid, recursively try to solve the rest of the puzzle
5. If no solution is found, backtrack and try the next number

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
