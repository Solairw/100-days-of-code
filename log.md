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

1. Learned what backtracking algorithms are. Such algorithm would solve any sudoku (if it doesn't have a mistake of course!). I will definetely try to implement one in future. Right now I try to stay with my current flow:
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

3. Done Bites of Py 103.

### Day 3: November 21, 2019

**Plan**: further sudoku solver development

**Today's Progress:**

1. The previous idea to improve algorithm kinda failed - at certain point the sudoku is filled in that way that the further solution is impossible. Trying to fix that by implying additional logic, for example turning problematic rows to their original condition.

2. Learned about `pdb.set_trace`. Useful for debugging porpuses!

3. Solved Bites of Py Exercises 104 and 105.

### Day 4: November 22, 2019

**Today's Progress:**

1. Solved Bites of Py Exercises 106 - 108

2. Learned a bit more about re module.

3. Learned about named tuples.

### Day 5: November 24, 2019

**Today's Progress:**

1. Solved Exercise 10 in Lerner's A3 course. Started creating config file.

2. Solved Bites of Py Excercises 109 and 110, thus finishing Intro section.

3. Solved Exercise 3 in Lerner's B3 course. Created a translator function replacing individual characters in string by another characters. Discovered `rpartition` function (https://stackoverflow.com/a/3675423/11321634):

```
def replace_last(source_string, replace_what, replace_with):
    head, _sep, tail = source_string.rpartition(replace_what)
    return head + replace_with + tail

s = "123123"
r = replace_last(s, '2', 'x')
print r
```

### Day 6: November 25, 2019

**Today's Progress:**

Solved Bites of Py 238 and 8. Today I learned about `unittest` while writing tests for Fibonacci number generator. Also learned about **Mutation testing** https://pypi.org/project/MutPy/.

### Day 7: November 26, 2019

**Today's Progress:**

Solved Bites of Py 15. Started PyBite 16.

### Day 8: November 27, 2019

**Today's Progress:**

Solved Bites of Py 16, 19.

### Day 9: November 28, 2019

**Today's Progress:**

Solved Bites of Py 21 and 26. Learned about dict comprehensions:
```
def filter_bites(bites=bites, bites_done=exclude_bites):
    """return the bites dict with the exclude_bites filtered out"""
    return {key:value for (key, value) in bites.items() if key not in exclude_bites}
```
### Day 10: November 30, 2019

**Today's Progress:**

Solved Bites of Py 29, 32, 37. Made first recursion function.

### Day 11: December 1, 2019

**Today's Progress:**

1. Solved Exercise 11 in Lerner's A3 course. Created Config class with backup functionality. Learned about `time()` function from `time` module- used for creating timestamps.

2. Started Exercise 4 in Lerner's B3 course. The task is to create zip file out of tar archive contents. File mteranipulation in Python is still tricky for me.

### Day 12: December 2, 2019

**Today's Progress:**

Solved Exercise 4 in Lerner's B3 course. It was tricky and tough. I got extra trouble since test file had a little mistake. However, I learned about `tarfile` and `zipfile` modules.

### Day 13: December 3, 2019

**Today's Progress:**

Solved Bites of Py 43 and 44.
Learned about forcing keyword arguments for functions:
```
def get_profile(*, name='julian', profession='programmer'):
    return f'{name} is a {profession}'
```
Learned about choices function in random module and string module:
```
def gen_key(parts=4, chars_per_part=8):
    return '-'.join([''.join(random.choices(string.ascii_uppercase + string.digits, k=chars_per_part))
                     for counter in range(parts)])
```
### Day 14: December 5, 2019

**Today's Progress:**

Solved Bites of Py 45 and 46.

### Day 15: December 7, 2019

**Today's Progress:**
Solved Exercise 12 in Lerner's A3 course. Learned about `__eq__`, `__gt__` and `__lt__` methods.

### Day 16: Decembber 8, 2019

**Today's Progress:**
1. Solved Exercise 5 in Lerner's B3 course. Made ImmutableMe class, which prevents user from mofiying attributes after object's instance creation and from adding new attributes.

2. Found an interesting project on Reddit. Started to explore the source code.
https://www.reddit.com/r/Python/comments/e735bt/this_is_an_open_invitation_to_anyone_who_wants_to/
Github link https://github.com/Jeremiah9000/Poker-with-Python
Youtube playlist with code explanation https://www.youtube.com/playlist?list=PLfGVDCs6poiOvs2UwPQ8vIZD4ilQElhAZ

### Day 17: December 9, 2019

**Today's Progress:**
Solved Bites of Py 54 and 55. Learned about `namedtuple` and `feedparser` module.


### Day 18: December 11, 2019

**Today's Progress:**
Solved Bites of Py 64 and 80.

### Day 19: December 13, 2019

**Today's Progress:**
Solved Bites of Py 66 and 74.

### Day 20: December 15, 2019

**Today's Progress:**
Solved Bites of Py 115 and 77.

### Day 21: December 17, 2019

**Today's Progress:**

Solved Exercise 13 in Lerner's A3 course. Created `__format__` method for Config class.

### Day 22: December 19, 2019

Solved Exercise 6 in Lerner's B3 course. Learned about `socket` module and created my first TCP server and client.

### Day 23: December 20, 2019

Solved parse_ranges Exercise in Python Morsels.

### Day 24: December 21, 2019

Solved Exercise 14 in Lerner's A3 course. Made `__enter__` and `__exit__` functions, thus making my first Context Manager!

### Day 25: December 23, 2019

Solved Bite of Py 143.

### Day 26: December 25, 2019

Solved Exercise 7 in Lerner's B3 course.

### Day 27: December 26, 2019

1. Solved Exercise 15 in Lerner's A3 course. Learned about `arrow` module and `attrgetter` method from `operator` module.

2. Solved Bite of Py 83. Learned about `pytz` module.

### Day 28: December 28, 2019

Solved Exercise 8 in Lerner's B3 course. Learned about `exec` function.

### Day 29: December 29, 2019

Worked on personal projects.

### Day 30: December 30, 2019

Worked on personal projects.

### Day 31: January 1, 2020

Solved Bite of Py 167.

### Day 32: January 3, 2020

Solved Bite of Py 218.

### Day 33: January 5, 2020

Solved Bites of Py 172 and 176.

### Day 34: January 7, 2020

Solved Bites of Py 169.

### Day 35: January 9, 2020

Solved Exercise 9 in Lerner's B3 course. Leaned about tinytag module.

### Day 36: January 11, 2020

Solved Bites of Py 91 and 180.

### Day 37: January 12, 2020

Solved Exercise 10 of Lerner's B3 course. Improved my knowledge of decorators.

### Day 38: January 14, 2020

Solved Bites of Py 189 and 208. Learned about `any` function. Also learned that `0.33 - 1 = -0.6699999999999999`

### Day 39: January 16, 2020

Worked on personal projects.
