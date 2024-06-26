# PRODIGY_SD_04

SODUKU SOLVER

    This python script implements a sudoku sover using backtracking algorithm. 
    
    The solver reads an input representing an unsolved Sudoku puzzle and fills in the missing numbers, adhering to Sudoku rules. 
    
    Once solved, the puzzle is printed.

  FEATURES 

    Board Representation:

      The Sudoku board is represented as a 2D list of integers. Zeros indicate empty cells.
    
    Printing the Board:

      The print_board(board) function prints the current state of the Sudoku board.

    Finding Empty Cells:

      The find_empty(board) function searches the board for empty cells (represented by 0) and returns their coordinates.

    Validation of Moves:

      The is_valid(board, num, pos) function checks whether placing a number in a specific position is valid according to Sudoku rules:
            
            The number must not already be present in the same row.
            
            The number must not already be present in the same column.
            
            The number must not already be present in the same 3x3 sub-grid.

    Solving the Puzzle:

      The solve(board) function uses a backtracking algorithm to solve the Sudoku puzzle. It tries placing numbers from 1 to 9 in each empty cell and recursively solves the rest of the board. If a placement leads to a dead end, it backtracks and tries the next number.
