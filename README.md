# Libft

A custom C library implementation of various standard library functions, created as part of the 42 School curriculum. This library provides essential functions for string manipulation, memory management, and linked list operations.

## 📚 Table of Contents
- [About](#about)
- [Function List](#function-list)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Testing](#testing)

## About

Libft is the first project at 42 School where students recreate various standard C library functions, along with additional utility functions that will be useful throughout the curriculum. This project helps understand the basic algorithms and data structures while implementing fundamental programming concepts.

## Function List

### Basic Functions (Libc)
| Function | Description |
|----------|-------------|
| ft_isalpha | Check if character is alphabetic |
| ft_isdigit | Check if character is digit |
| ft_isalnum | Check if character is alphanumeric |
| ft_isascii | Check if character is ASCII |
| ft_isprint | Check if character is printable |
| ft_strlen | Calculate string length |
| ft_memset | Fill memory with a constant byte |
| ft_bzero | Zero a byte string |
| ft_memcpy | Copy memory area |
| ft_memmove | Copy memory area with overlap handling |
| ft_strlcpy | Size-bounded string copying |
| ft_strlcat | Size-bounded string concatenation |
| ft_toupper | Convert char to uppercase |
| ft_tolower | Convert char to lowercase |
| ft_strchr | Locate character in string |
| ft_strrchr | Locate character in string from the end |
| ft_strncmp | Compare two strings |
| ft_memchr | Scan memory for a character |
| ft_memcmp | Compare memory areas |
| ft_strnstr | Locate a substring in a string |
| ft_atoi | Convert string to integer |
| ft_calloc | Allocate and zero-initialize memory |
| ft_strdup | Create a duplicate of a string |

### Additional Functions
| Function | Description |
|----------|-------------|
| ft_substr | Create substring from string |
| ft_strjoin | Concatenate two strings |
| ft_strtrim | Trim characters from string |
| ft_split | Split string into array of substrings |
| ft_itoa | Convert integer to string |
| ft_strmapi | Apply function to each char of string |
| ft_striteri | Apply function to each char of string with index |
| ft_putchar_fd | Output char to file descriptor |
| ft_putstr_fd | Output string to file descriptor |
| ft_putendl_fd | Output string with newline to file descriptor |
| ft_putnbr_fd | Output number to file descriptor |

### Bonus Functions (Linked Lists)
| Function | Description |
|----------|-------------|
| ft_lstnew | Create new list node |
| ft_lstadd_front | Add node at beginning of list |
| ft_lstsize | Count nodes in list |
| ft_lstlast | Get last node of list |
| ft_lstadd_back | Add node at end of list |
| ft_lstdelone | Delete node with specific deleter |
| ft_lstclear | Delete list with specific deleter |
| ft_lstiter | Apply function to all list nodes |
| ft_lstmap | Create new list by applying function |

## Getting Started

### Prerequisites
- GCC compiler
- Make

### Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/Libft.git
cd Libft
```

2. Compile the library:
```bash
make        # Compile mandatory functions
make bonus  # Compile with bonus functions
```

This will create `libft.a` static library.

## Usage

1. Include the header in your C file:
```c
#include "libft.h"
```

2. When compiling your program, link the library:
```bash
cc your_program.c -L. -lft
```

### Example
```c
#include "libft.h"

int main(void)
{
    char *str = "Hello, 42!";
    if (ft_isalpha(str[0]))
        ft_putstr_fd("First character is alphabetic\n", 1);
    return (0);
}
```

## Testing
You can test the library using any of these popular testing tools:
- [Tripouille/libfttester](https://github.com/Tripouille/libfttester)
- [alelievr/libft-unit-test](https://github.com/alelievr/libft-unit-test)
- [jtoty/Libftest](https://github.com/jtoty/Libftest)

## Cleaning
```bash
make clean    # Remove object files
make fclean   # Remove object files and library
make re       # Recompile library
```

---
Created as part of 42 School curriculum
