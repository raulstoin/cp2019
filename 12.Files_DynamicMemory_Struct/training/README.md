## Files, Dynamic memory allocation, Structures

### Task 1
Write a program that reads a database of students from a given file, sorts the students descending by grades, and prints the sorted data to another given file. File names (paths) are given as command line arugments (e.g. **./prog infile.txt outfile.txt**).

The format of the database:

- one student entry per line
- an entry is a tuple: (id lastName grade)
- database number of entries is unknown.

### Task 2 - Splitting into words (M. Minea)
Write a function that splits a string into words (strings with no whitespace), returning a (dynamically allocated) array of pointers to (dynamically allocated) copies of the words in the string.

### Task 3 - Split lines
Read text from a given file as command line argument and split lines longer than 1024 characters. Store the text in memory as array of pointers to lines. Each line is stored as a structure type, consisting in a string (the text on the line) and the line length.

