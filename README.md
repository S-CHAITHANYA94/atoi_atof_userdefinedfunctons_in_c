Here is a clean README.md for your atoi and atof repository:

Atoi and Atof Implementation in C

This repository contains custom implementations of "atoi()" and "atof()" functions in C. The project demonstrates how strings containing integer and floating-point numbers can be converted into numeric values without directly using the standard library conversion functions.

Files

- "atoi.c" – Custom implementation of "atoi()"
- "atof.c" – Custom implementation of "atof()"
- "main.c" – Takes string input and automatically calls "my_atoi()" or "my_atof()"
- "LICENSE" – Unlicense

Features

- Converts a string into an integer using "my_atoi()"
- Converts a string into a floating-point value using "my_atof()"
- Handles positive and negative numbers
- Skips spaces and double quotes at the beginning
- Detects whether the input is an integer or floating-point number
- Demonstrates string processing using character-by-character conversion

How It Works

"my_atoi()"

The "my_atoi()" function converts numeric characters from a string into an integer.

For example:

Input:  -12345
Output: -12345

The conversion is performed using:

num = num * 10 + r;

where "r" is the numeric value of the current character.

"my_atof()"

The "my_atof()" function converts a string containing a floating-point number into a "double".

For example:

Input:  123.456
Output: 123.456000

The digits before the decimal point are processed as the integer part, while digits after the decimal point are divided by "10", "100", "1000", and so on.

Compilation

Compile the program using GCC:

gcc main.c atoi.c atof.c

Run the program:

./a.out

Example

Integer Input

Enter a string:
-12345

-12345

Floating-Point Input

Enter a string:
-123.456

-123.456000

Concepts Used

- C functions
- Strings
- Character arrays
- Pointers
- Loops
- Conditional statements
- ASCII character values
- Type conversion
- Integer arithmetic
- Floating-point arithmetic
- Modular programming
- Multi-file compilation

Learning Objective

The main objective of this project is to understand how standard string-to-number conversion functions can be implemented manually in C. It also provides practice with pointers, strings, functions, loops, and floating-point calculations.

License

This project is released under the Unlicense, meaning it is dedicated to the public domain as far as legally possible. 