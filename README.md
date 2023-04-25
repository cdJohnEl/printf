## ALX Printf Project.
**This is a collaborative project to implement the printf function in C programming language. The printf function is used to print output to the console in a specific format. This project is a significant part of the curriculum for the ALX Software Engineering program.**

## Synopsis.
**int _printf(const char *format, ...);** is the protype of the function, and this implies that the function takes one madatory argument that can not be altered, since it's a const, and some optional varying number of arguments. The content of the string format determines what happens to the other argument(s), if any.

**_printf()** was written to use a local buffer of 1024 bytes when printing although it can print larger sets of data. Its return value ( after a successful execution) is the total number of characters printed to stdout, or -1 if an output error is encountered.

_printf() is supposed to print every character that is within the double quotes (in the string) to stdout, except special characters, such as format specifiers that is preceded by '%', which initiates some conversion that will involve some optional argument(s).

A conversion specifier usually follows the '%', which determines the exact conversion to be made. Between the percentage symbol (%) and the conversion specifier, there may be (in the following order):

Zero or more flags

An optional field width

## Features.
Our implementation of the printf function supports the following format specifiers:

%c - prints a single character.
%s - prints a string of characters.
%d - prints a signed decimal integer.
%i - prints a signed decimal integer.
%u - prints an unsigned decimal integer.
%x - prints a hexadecimal integer (lowercase).
%X - prints a hexadecimal integer (uppercase).
%o - prints an octal integer.
%b - prints a binary integer.
%p - prints a pointer address.
%% - prints a literal % character.

**In addition, the following flags and modifiers are supported:**

\- - left-justify the output.
\+ - always print a sign (+ or -) for signed integers.
0 - pad with zeros instead of spaces.
\# - print the prefix (0 or 0x) for octal/hexadecimal numbers.
(space) - prefix positive signed integers with a space.
\. - specify the precision for floating-point numbers.

Our implementation of printf is also capable of handling custom format specifiers, which allows the user to define their own format specifiers for special use cases.

## Installation and Testing

Simply clone the repository by copying the code below to clone the repository on your local machine (Linux distro)

git clone https://github.com/Easykeljohn/printf.git.

After cloning, navigate into the directory printf and write a main.c file to test **_printf()**, and then compile, probably with the command gcc *.c -o _printf and run the file **(./_printf)**

Alternatively,the sub directory test_files contains a main file and an executable named main that will be available on your local machine after cloning the repository, you may take a look at the source code and run the executable to see the output. You may as well modify the content of the main.c, copy it to the root directory and recompile

Submitted by: [John Chimdike Ezekiel](https://github.com/Easykeljohn) and [Nnenna Nkata](https://github.com/nellyrobert)
