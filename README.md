# _printf
The `printf` is a collection of C files that when compiled and executed, produces output according to a format. It replicates the standard `printf()` function. This project was to be done in a group of two (pair programming).

# Requirements
* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be compiled on Ubuntu 20.04 LTS using `gcc`, using the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
* All your files should end with a new line
* A `README.md` file, at the root of the folder of the project is mandatory
* Your code should use the `Betty` style. It will be checked using [betty-style.pl](https://github.com/holbertonschool/Betty/blob/master/betty-style.pl) and [betty-doc.pl](https://github.com/holbertonschool/Betty/blob/master/betty-doc.pl)
* You are not allowed to use global variables
* No more than 5 functions per file
* The prototypes of all your functions should be included in your header file called `main.h`
* Don’t forget to push your header file
* All your header files should be include guarded
* Note that we will not provide the `_putchar` function for this project

# More Info
## Authorized functions and macros
* `write (man 2 write)`
* `malloc (man 3 malloc)`
* `free (man 3 free)`
* `va_start (man 3 va_start)`
* `va_end (man 3 va_end)`
* `va_copy (man 3 va_copy)`
* `va_arg (man 3 va_arg)`

# Compilation
* Your code will be compiled this way:
``$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c``
* As a consequence, be careful not to push any c file containing a `main` function in the root directory of your project (you could have a `test` folder containing all your tests files including main functions)
* Our main files will include your main header file (`main.h`): `#include main.h`
* You might want to look at the gcc flag `-Wno-format` when testing with your `_printf` and the standard `printf`.

## Prototype of _printf function
`int _printf(const char *format, ...);`
Returns: the number of characters printed (excluding the null byte used to end output to strings)

## Usage
* Include main.h
* Call `_printf`, passing a formatted string with any format specifiers and optional arguments
* Upon success, it writes desired output to stdout
* Upon error, it returns -1
* If NULL is passed in as a string argument, it prints `(null)`

## Format Specifiers
| Format Specifier | Description | Function name |
| ---- | ------ |------|
| `%c` | Prints a character | `print_c` |
| `%s` | Prints a string | `print_s` |
| `%X` | Prints a char's ascii value in uppercase hex | `hex_print` |
| `%S` | Prints a string and nonprintable character ascii values | `print_S` |
| `%r` | Prints astring in reverse | `print_r` |

## Example Usage
* `printf("%c", 'd')` -  Prints the character `d`
* `printf("%s", "Hello, world\n")` - Prints "Hello, world", followed by a new line

# Tasks
Projects table




## Authors
* [Wolleys Migaya](https://github.com/Wolleys)
* [Zumrati Yusuf](https://github.com/zumrati)
