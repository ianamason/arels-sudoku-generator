# Arel's Sudoku Generator
A simple sudoku generator written in Python in 2005, before I knew about linting, apparently.

This is an archive of a script described here: https://www.ocf.berkeley.edu/~arel/sudoku/main.html

![demo-image](https://user-images.githubusercontent.com/153497/83680961-b0a9cf80-a5af-11ea-81f2-39ca1e4a62be.png)

Sudoku is a logic based placement puzzle, also known as Number Place in the United States. The aim of the puzzle is to enter a numerical digit from 1 through 9 in each cell of a 9*9 grid made up of 3*3 subgrids (called "regions"), starting with various digits given in some cells (the "givens"). Each row, column, and region must contain only one instance of each numeral. Completing the puzzle requires patience and logical ability. Its grid layout is reminiscent of other newspaper puzzles like crosswords and chess problems. Although first published in 1979, Sudoku initially became popular in Japan in 1986 and attained international popularity in 2005. [Read more...](http://en.wikipedia.org/wiki/Sudoku)

Below is a simple program written to generate Sudoku puzzles. It was written in python (in the matter of a few hours so please excuse its inelegance). To run it, just type python sudoku.py at the command line or use your favorite python interpreter.
Creating (and solving) these puzzles is a constraint satisifaction problem, which in general is a hard thing. However, this program takes advantage of the fact that most CSPs aren't hard in the average case.

## Generating a puzzle

* Python 2.x is required.

```bash
$ python2 sudoku.py

Constructing a sudoku puzzle.
* creating the solution...
* constructing a puzzle...
7 8 _ _ _ 4 _ _ _
_ _ 6 5 _ _ _ _ _
_ 2 _ _ _ 6 9 3 1
3 9 _ _ 1 _ 4 7 _
_ _ _ 2 5 _ _ _ 9
_ _ _ _ _ _ _ 6 _
9 _ _ _ 8 _ 3 4 _
_ 7 1 _ _ 5 2 _ _
8 6 _ 4 2 _ _ 5 _

```
