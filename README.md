# calculator

A task to practice programming by creating a BC-like calculator

## Task

Create a [bc](https://www.gnu.org/software/bc/manual/html_mono/bc.html) clone command line application with a limited feature set, that can evaluate mathematical expressions.

1. The tool should have a command prompt for the user inputs that are mathematical expressions.
2. The tool should validate the expression and print an error with details of the expression error to the console (character, position, reason).
3. The tool should print the result of valid expressions to the console.
4. The tool should request input until it is terminated or the `quit` command/input is passed to it.
5. It should support literals of **numbers**:
   1. Integer numbers, e.g. `42`
   2. Fractional numbers, e.g. `4.2`
   3. Positive and negative numbers, e.g. `-42`, `+4.2`
   4. Shorthand fractional numbers, e.g. `.3` equals `0.3`, `42.` equals `42.0`
   5. Leading zeros for the integer part, e.g. `00042` equals `42`
   6. Trailing zeros for the fractional part, e.g. `42.1000` equals `42.1`
   7. Numbers by science notation, e.g. `-3.2e5` equals `-320000`
   8. Decimal separators (`,`, `_`), e.g. `3,456.11` equals `3456.11`
   9. Literals cannot have white space in them, e.g. `3 456.5` is not valid
6. It should support **operators**:
   1. Addition, e.g. `42 + 13` equals `55`
   2. Subtraction, e.g. `42 - 13` equals `29`
   3. Multiplication, e.g. `42 * 2` equals `84`
   4. Division, e.g. `42 / 4` equals `10.5`
   5. Integer division, e.g. `42 // 4` equals `10`
   6. Modulo, e.g. `42 % 4` equals `2`
   7. Power, e.g. `2 ^ 3` equals `8`
   8. Operations can be grouped, e.g. `(12 + 3) * 2` equals `30`
   9. There can be any white space between the operator and the operands until the expression is deterministic.
   10. Operators should have the following precedence (highest to lowest, Left-to-right on the same level):
       1.  Grouping
       2.  Power, Modulo, Integer division, Division, Multiplication
       3.  Addition, Subtractioní

## Technology

Use any technology and programming language you wish.

## Test

Implement your tests, using the test data available in `test_data.json`, which contains an array of test data records:
* `input`: one line of input to the tool
* `output`: the output for the input line, unless there is an error
* `error`: the error displayed on the screen if expected

Note, that these are not all the possible test cases, feel free to add yours.