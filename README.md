# ft_printf Project

## Overview

This project is my 2th project at School 42. This project aims to create a custom implementation of the printf function, named ft_printf(), which mimics the behavior of the original [printf()](https://man7.org/linux/man-pages/man3/printf.3.html) function from the C Standard Library (libc). The goal is to recode the printf() function, handling various format specifiers, without implementing the buffer management of the original printf().

# Prototype
```c
int ft_printf(const char *, ...)
```

# Usage

```c
#include "ft_printf.h"  // Include the header file for ft_printf function

int main() {
    // Example usage of ft_printf
    ft_printf("Hello, %s! Your number is %d and in hexadecimal it is: %x\n", "User", 42, 42);

    // You can also use printf for comparison
    printf("Hello, %s! Your number is %d and in hexadecimal it is: %x\n", "User", 42, 42);

    return 0;
}
```

## Makefile targets

- Makefile Targets
- NAME: Specifies the name of the output library.
- all: Builds the ft_printf library.
- clean: Removes object files.
- fclean: Removes object files and the ft_printf library.
- re: Executes fclean and then rebuilds the library.

## External Functions

- malloc
- free
- write
- va_start
- va_arg
- va_copy
- va_end

## Implemented Conversions
The following conversions are implemented in ft_printf():

- %c: Prints a single character.
- %s: Prints a string as defined by the common C convention.
- %p: Prints a void * pointer argument in hexadecimal format.
- %d: Prints a decimal (base 10) number.
- %i: Prints an integer in base 10.
- %u: Prints an unsigned decimal (base 10) number.
- %x: Prints a number in hexadecimal (base 16) lowercase format.
- %X: Prints a number in hexadecimal (base 16) uppercase format.
- %%: Prints a percent sign.

## Installation

Clone the repository:

```bash
git git@gitlab.com:dinis-petrukha/ft_printf.git ft_printf
cd ft_printf
```

Execute the Makefile:
```bash
make
```
Feel free to explore and contribute to the project!