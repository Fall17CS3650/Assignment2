# Assignment2

## Information

Please edit the following information in your assignment

Name:

How many hours did it take you to complete this assignment?

Did you collaborate with any other students/TAs/Professors?

(Optional)
What was your favorite part of the assignment?
How would you improve the assignment?


# Assignment

In this assignment, you will be getting some familiarity with working with the C programming language.

## Section 1 - C Programming

You will write two different .c files and compile them with clang. The files will be lower case and named exactly.

### Part 1 - Sorting integers
You will be sorting a list of integers. 

1. Create a file called ints.c
2. Your program will generate N number of random integers.
3. Look to the stdlib.h library for generating random numbers.
4. Your program will read from the command line an argument for how many random numbers to generate and sort
5. Because it is not known at compile time, you will have to allocate an array of integers using malloc. An example of malloc for the char datatype is here: [http://www.cplusplus.com/reference/cstdlib/malloc/]. Do not forget to free your memory at the end of the program!

Test your program by compiling it: `clang ints.c -o ints`

Run your program using the following: `./ints 100`

### Part 2 - Sorting Strings

You will be sorting a list of strings. 

1. Create a file called strings.c
2. Your program will read in a file called test1.txt
3. test1.txt contains several ascii strings that you will sort.
4. It will be helpful to understand the strcmp function. [http://www.cplusplus.com/reference/cstring/strcmp/]
5. Because it is not known at compile time, you will have to allocate an array of strings using malloc. An example of malloc for the char datatype is here: [http://www.cplusplus.com/reference/cstdlib/malloc/]. Do not forget to free your memory at the end of the program!

Test your program by compiling it: `clang strings.c -o strings`

Run your program using the following: `./strings test1.txt`

## Section 2 - More Terminal Tricks

Part of this course is getting comfortable in the termainal.

1. ssh into username@login.ccs.neu.edu
2. Run the command 'cat /proc/cpuinfo'
3. Pipe this to a file called proc.txt and commit it to the repo.

proc itself is a pseudo-file system. So the information we are outputting is information that is gathered at runtime (i.e. when you are running a system).

1. Now run the command 'lscpu' this will display information about our computer architecture. Our architecture on the ccs machines should be x86_64--otherwise we will have trouble proceeding in this course!
2. Pipe this information to a file called lscpu.txt.

Here is one bonus command.

1. As a bonus, run the command 'top'
2. See if any of your classmates in the USER list are also logged into the ccs machines at this time!

## Rubric

1. 5% for completing the README
2. 5% for completing Section 2 - More Terminal Tricks
3. 45% for completing the sorting of integers
4. 45% for completing the sorting of strings given an input file.

Notes:

1. programs that do not compile get 0%
2. Your program should not leak memory. [https://www.ibm.com/developerworks/aix/library/au-toughgame/index.html]
3. Your program(s) should handle edge cases (e.g. an empty list is passed in, a list of words that are all the same, a negative integer is passed in). You may assume all inputs are words using lower-case characters (a-z).
4. You should have comments in your code to explain what is going on, and use good style (80 characters per line maximum for example, functions that are less than 50 lines, etc.).


## Glossary and Tips

Compile-Time: The program before it is actually running. Some information is not known, for example what program arguments are being read from the command line.

Runtime: The state the program is in when it is actually executing.

### Tips
1. Commit your code changes to the repository often, this is best practice.
2. Do not commit your .o file or your executable file to the repository, this is considered bad practice!
