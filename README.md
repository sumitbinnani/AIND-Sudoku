# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: *The naked twins strategy looks for two boxes with identical values in the same unit. Given {'A1': '13', 'B1':'13',  ...} for first columnar unit, we can conclude that 1 and 3 must be in A1 and B1 (although we don't know which is where). We can thus eliminate 1 and 3 from all the boxes in the unit containing this twin boxes (top-left square unit in the example under consideration). The only_choice strategy would now have stricter constraints to fill in the other boxes in square and might lead to further solving.*

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: *Diagonal sudoku can be implemented by addition of two extra diagonal units to account for diagonal constraints. The same code will iterate through all the units, and the constarints would thus propogate.*

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.