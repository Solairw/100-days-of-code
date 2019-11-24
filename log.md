# 100 Days Of Code - Log

### Day 0: November 19, 2019

**Plan**: study Github tutorial, do code

**Today's Progress**: 

1. Passed GitHub tutorial (again!). Uploaded my project (sudoku_solver). I will be developing it further. 

2. Today, I added function to check if the solution submitted by user is correct or not (the validator).

3. Solved two Bites of Py Exercises (101 and 102).

**Thoughts:** Progress is not much, but this is just the beginning.

**Link to work:** [Sudoku_solver](https://github.com/Solairw/sudoku_solver)

### Day 1: November 20, 2019

**Plan**: learn what is my current algorithm lacking and find paths for future development.

**Today's Progress**:

1. Learned what are backtracking algorithms are. Such algorithm would solve any sudoku (if it doesn't have a mistake of course!). I will definetely try to implement one in future. Right now I try to stay with my current flow:
  1. Find possible solution for every cell.
  2. Find which cells have only one possible solution and fill them.
  3. Return to 1.
  4. Voila - a solved sudoku!
However, there are harder sudokus where there are multiple possible solutions on each cell (at least at the beginning). Thus, my task is to implement the following algorithm:
      1. Find possible solution for every cell.
      2. *Do something*.
      3. Voila - a solved sudoku!
I have not yet discovered how to do Step 2 yet. I don't want to get a solution from Internet and want to try complete this challenge for myself. Tried to do some code, pushed it to `better_solver` branch on GitHub.

2. Completed Sudoku Solution Validator on Codewars https://www.codewars.com/kata/529bf0e9bdf7657179000008

3. Done Bites of Py Exercise 103.

### Day 3: November 21, 2019

**Plan**: further sudoku solver development

**Today's Progress:

1. The previous idea to improve algorithm kinda failed - at certain point the sudoku is filled in that way that the further solution is impossible. Trying to fix that by implying additional logic, for example turning problematic rows to their original condition.

2. Learned about `pdb.set_trace`. Useful for debugging porpuses!

3. Solved Bites of Py Exercises 104 and 105.

### Day 4: November 22, 2019

**Today's Progress:

1. Solved Bites of Py Exercises 106 - 108

2. Learned a bit more about re module.

3. Learned about named tuples.

### Day 5: November 24, 2019

**Today's Progress:

1. Solved Excercise 10 in Lerner's A3 course. Started creating config file.

2. Solved Bites of Py Excercises 109 and 110, thus finishing Intro section.
