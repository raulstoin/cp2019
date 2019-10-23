# Input processing

### Task 1
Given a text on multiple lines at standard input, print all decimal numbers that can be found in the text. If whitespaces are encountered, compact all adiacent ones and print a space (' ') character instead, except newline (which shall be kept as it is). The program should stop when the entire text has been processed.

| Input                                               | Output  |
|---                                                  |---      |
|123abc23a&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;567ab   | 123 23 567 |
|asdg456&nbsp;&nbsp;&nbsp;asd356                      | 456 356 |
|3579ah&nbsp;&nbsp;                                   | 3579    |

### Task 2
Given a text on multiple lines at standard input, print all numbers that can be found in the text in base 8, base 10, or base 16. Skip all other characters. Rules of base notation:
- a number in base 8 starts with 0 and can be followed by [0-7]
- a number in base 10 starts a digit [1-9] and can be followed by any digits [0-9]
- a number in base 16 starts with 0x and must be followed by at least one hexdigit ([0-9] , [A-F], [a-f] ), then any number of hexdigits.

The program should stop when the entire text has been processed or an invalid number was detected (e.g. 01238, 0xG, 1A etc).

