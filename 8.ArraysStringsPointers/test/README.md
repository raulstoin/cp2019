# Arrays, strings, pointers - test

### Task 1 - The beginning of the vowels...
Implement a function ***vowelWords(s, v, n)*** that stores all the indexes of words that start with a vowel from string **s** in array **v**, but no more than **n** elements. The function should return the actual number of elements stored in array **v**. Prove that your code works by calling the function in main.

Notes:
- DO NOT USE **strtok**!
- Function arguments:
  - **s** - the given string
  - **v** - an array of integers, where the indexes of words should be stored
  - **n** - the maximum capacity of array **v**, which must not be exceeded when storing the values.
- The index of a word is the position in string of the first character of the word.
- A word is defined as a sequnce of non-whitespace characters separated by whitespaces (except the first and last words).

### Task 2 - Censorship

Write a program which receives arguments in main from console and prints all argument values which have a length smaller or equal than the largest word in the argument list. Replace all these words contents with **#** character (as many as the string length).

Notes:
- header for main should be **int main(int argc, char \*argv[])**

