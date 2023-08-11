# Wordle Solver

A sophisticated Wordle game solver grounded in Information Theory. Using an advanced algorithm, it dynamically calculates the expected entropy of each word based on previous guesses, to optimize subsequent guesses. This project also includes an interactive graphical interface in pygame, which displays the 10 best guesses, and the corrosponding expected amount of information gained.

## Features

**Information Theory Based Algorithm:** Improves guess accuracy by computing the expected entropy of each word.

**Interactive GUI:** Displays the top 10 word predictions dynamically.

**Performance:** Achieves an average score of ~3.44.

## Installation

1. **Prerequisite**: Ensure you have [Python](https://www.python.org/downloads/) installed on your machine.

2. **Dependency**: This project requires the `pygame` module. You can install it using pip:

```bash
pip install pygame
```

If you're new to pygame, you can read more about it and its installation [here](https://www.pygame.org/wiki/GettingStarted).

**Clone the repository:**
```bash
git clone https://github.com/Jackelelelelele/Wordle-Solver.git
```

## Usage

Type in a 5 letter word and hit **Enter** to input a guess, use **Backspace** to delete a letter. Invalid words will not be accepted. The best guesses ranked are listed on the right side of the screen.

**NOTE:** Occasionally on the initial guess, the program might take longer to process a word, this occurs in instances where the initial guess provides very little info (such as 5 greys). Please be patient and wait for the code to execute during such instances. I'm currently working on optimizing the code for future updates to reduce these delays.

## Datasets
The solver utilizes several text files to function:

**fullwordlist.txt:** Contains all possible words that can be inputted as guesses.

**wordleanswers.txt:** A compilation of all potential answers, matching the list used by The New York Times.

**wordlecombinations.txt:** Additional data used by the solver for its computations.
