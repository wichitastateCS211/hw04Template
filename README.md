# Rolling Dice
Simulate rolling a six-sided die 500,000 times and chart the results.

## Requirements
- The program does not take any input.
- Roll the die 500,000 times and keep a tally of the results.
- In order for the chart to fit easily on the screen, each asterisk must represent 5,000 rolls (1% of the total rolls) of a given value.
- Two functions are required:
  - `int roll_d6()`
    - Return: the result of a random roll of a six-sided die.
    - Parameters: N/A
  - `void print_table_row(int val, int numValRolls, int totalNumRolls)`
    - This function will only print a single row of the table seen in the sample run. For example, calling it
      `print_table_row(1, 83320, 500'000)` will print the row of table that shows how many 1s were rolled. The
      function is **not** responsible for printing the table header.
      - **NOTE:** You won't be calling the function exactly like this, i.e., you won't be using all literals.
    - Return: N/A
    - Parameters:
      - `int val`: the die face being represented
      - `int numValRolls`: The number of rolls that were equivalent to `val`.
      - `int totalNumRolls`: The total number of dice rolls.

## Sample Run
Your distribution may not look exactly like this, but all bars should be very nearly
equivalent with each other to represent a fair die.

```
Distribution of dice rolls
==========================
1: ****************
2: ****************
3: ****************
4: ****************
5: ****************
6: ****************
```

## Hints
- The objects required to generate random numbers should not be re-initialized every time the function `roll_d6()` is called.
  - Ask me about `static` in class.
- The total number of rolls should not be a magic number.
- Integer division is sufficient.
- While two functions are required, you may write additional functions if they suit your solution.

## Reminders
- Name your file *wsuid*\_hw04.cpp
- You are required to place a comment block at the top of the file. Refer to the Coding Guidelines
handout.
