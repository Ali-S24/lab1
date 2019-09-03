# Lab 1.1: Separate compilation

Write a .h/.cpp module pair named ```intfuncs``` containing several functions operating on integers:

   * ```min```: accept two integers and return their minimum (as an integer)
   * ```max```: accept two integers and return their maximum (as an integer)
   * ```average```: accept two integers and return their average (as a double)
   * ```abs```: accept a single integer and return its absolute value

Write an application ```intfuncs_app.cpp``` that accepts pairs of integers from the keyboard (until eof) and runs each function on each pair.

Sample test run:

```
first number? 2
second number? 4
The maximum of 2 and 4 is 4
The minimum of 2 and 4 is 2
The average of 2 and 4 is 3
The absolute value of 2 is 2
The absolute value of 4 is 4

first number? 7
second number? 4
The maximum of 7 and 4 is 7
The minimum of 7 and 4 is 4
The average of 7 and 4 is 5.5
The absolute value of 7 is 7
The absolute value of 4 is 4

first number? 6
second number? -1
The maximum of 6 and -1 is 6
The minimum of 6 and -1 is -1
The average of 6 and -1 is 2.5
The absolute value of 6 is 6
The absolute value of -1 is 1

first number?

```

# Lab 1.2: Parameter transmission
Having call-by-reference allows one to use storeback parameters, i.e., parameters whose values are transmitted back to their arguments. In this exercise, you are to write a program that provides several variations of a function that calculates the minimum of two values. Several of the functions also report whether the two values passed in were equal. The functions are all named ```min``` — they differ in their arguments and return values:

   * Accept two integers and return their minimum
   * Accept three parameters: two integers, and a third integer storeback set to the minimum of the first two. Return a boolean set to true if the inputs are _not_ equal, and false otherwise.
   * Accept three parameters: two integers, and a boolean storeback set to true if they are _not_ equal and false otherwise. Return an integer set to the minimum of the two inputs.
   * Accept four parameters: two integers, a boolean storeback set to true if they are not equal and false otherwise, and another integer storeback set to the minimum of the two. 

Call the file ```min.cpp```. In the same file, write a ```main``` function demonstrating use of the above functions. The app should accept pairs of integers from the console (until eof), call each of the function sand print out the results using the format illustrated below:

Sample test run:
```
first number? 3
second number? 4
int min(x, y): The minimum of 3 and 4 is 3
bool min(x, y, min): The minimum of 3 and 4 is 3
int min(x, y, ok): The minimum of 3 and 4 is 3
void min(x, y, ok, min): The minimum of 3 and 4 is 3

first number? 5
second number? 2
int min(x, y): The minimum of 5 and 2 is 2
bool min(x, y, min): The minimum of 5 and 2 is 2
int min(x, y, ok): The minimum of 5 and 2 is 2
void min(x, y, ok, min): The minimum of 5 and 2 is 2

first number?

```

# Grading
The following factors will be part of this lab's grade:

   * Compilation: the code must compile (check Travis)
   * Style: indentation, variable naming, comments (make sure indentation survives uploading to github)
   * Compliance: all files and functions must be named as specified in the instructions, all output must look as specified
   * Correctness: all behavior specified in the readme must be implemented correctly

# Policies

## Collaboration
Discussion and working together is permitted. However, *submitted code must not be identical* and identical code will be considered plagiarism.

## Revision
Submissions may be revised until the due date, even after a pull request has been submitted, and even after an early submission has been graded.
