# Arrays, strings, pointers

### Task 1 - String compare
Implement your own versions of strcmp and strncmp (with the exact same functionality).

### Task 2 - Definitions in strings
Write a function that takes a string, prints all definitions of the form ***name*=*value*** from the string, one per line, and returns their number. The ***name*** must be an identifier (like in C: starts with letter or underscore, may contain letters, underscore and digits). The ***value*** may contain arbitrary non-whitespace. Definitions must be separated by whitespace from other parts of the string.

### Task 3 - Ints in string
Write a function that prints out all numbers (strings of digits with optional sign) from a string given as parameter. Consider only standalone numbers, i.e. numbers that do not have any non-whitespace characters adjacent to them.

### Task 4 - Ints positions in string
Write a function that stores pointers to all numbers (strings of digits with optional sign) from a string given as parameter into an array of pointers given as parameter (a pointer to a number should point at each number's beginning). The maximum capacity of the array will be received as another argument called **maxCap** and it must not be exceeded when filling the array (store up to **maxCap** pointers). Consider only standalone numbers, i.e. numbers that do not have any non-whitespace characters adjacent to them.

### Task 5 - Define and replace
Write a funcion that receives a string, identifies the first line of the form **#define somename restofline** (where somename is a C identifier), separated left and right by whitespace, and prints the remaining input substituting any standalone occurrence of **somename** with **restofline**. Emulate multiple lines by using **\n** in your string.

E.g.: 
```C
#define ABCD ef123 - 12
some data
x= ABCD
y = x + ABCD * 4
```
to
```C
some data
x= ef123 - 12
y = x + ef123 - 12 * 4
```

### Task 6 - Input arguments parser

Write a function called ***filterArgs*** that receives the entire program argument list from *main* (argc and argv) and prints out only pairs of correct options starting from *argv[1]*. A correct option pair is defined as follows:
* *dash* + *letter* + *whitespaces* (at least 1) + *a sequence of non-whitespace characters*
  - i.e. **-o prog1234**
- *double dash* + *a sequence of letters* + *equal* (=) + *a sequence of non-whitespace characters*
   - i.e. **\-\-compress=max-optimize_2**

Note: The sequence of non-whitespace characters cannot start with a dash, i.e. **-o -prog** is not a valid option pair!

