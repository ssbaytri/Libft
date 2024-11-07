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
| [`ft_isalpha`](libft/ft_isalpha.c) | Check if character is alphabetic |
| [`ft_isdigit`](libft/ft_isdigit.c) | Check if character is digit |
| [`ft_isalnum`](libft/ft_isalnum.c) | Check if character is alphanumeric |
| [`ft_isascii`](libft/ft_isascii.c) | Check if character is ASCII |
| [`ft_isprint`](libft/ft_isprint.c) | Check if character is printable |
| [`ft_strlen`](libft/ft_strlen.c) | Calculate string length |
| [`ft_memset`](libft/ft_memset.c) | Fill memory with a constant byte |
| [`ft_bzero`](libft/ft_bzero.c) | Zero a byte string |
| [`ft_memcpy`](libft/ft_memcpy.c) | Copy memory area |
| [`ft_memmove`](libft/ft_memmove.c) | Copy memory area with overlap handling |
| [`ft_strlcpy`](libft/ft_strlcpy.c) | Size-bounded string copying |
| [`ft_strlcat`](libft/ft_strlcat.c) | Size-bounded string concatenation |
| [`ft_toupper`](libft/ft_toupper.c) | Convert char to uppercase |
| [`ft_tolower`](libft/ft_tolower.c) | Convert char to lowercase |
| [`ft_strchr`](libft/ft_strchr.c) | Locate character in string |
| [`ft_strrchr`](libft/ft_strrchr.c) | Locate character in string from the end |
| [`ft_strncmp`](libft/ft_strncmp.c) | Compare two strings |
| [`ft_memchr`](libft/ft_memchr.c) | Scan memory for a character |
| [`ft_memcmp`](libft/ft_memcmp.c) | Compare memory areas |
| [`ft_strnstr`](libft/ft_strnstr.c) | Locate a substring in a string |
| [`ft_atoi`](libft/ft_atoi.c) | Convert string to integer |
| [`ft_calloc`](libft/ft_calloc.c) | Allocate and zero-initialize memory |
| [`ft_strdup`](libft/ft_strdup.c) | Create a duplicate of a string |

### Additional Functions
| Function | Description |
|----------|-------------|
| [`ft_substr`](libft/ft_substr.c) | Create substring from string |
| [`ft_strjoin`](libft/ft_strjoin.c) | Concatenate two strings |
| [`ft_strtrim`](libft/ft_strtrim.c) | Trim characters from string |
| [`ft_split`](libft/ft_split.c) | Split string into array of substrings |
| [`ft_itoa`](libft/ft_itoa.c) | Convert integer to string |
| [`ft_strmapi`](libft/ft_strmapi.c) | Apply function to each char of string |
| [`ft_striteri`](libft/ft_striteri.c) | Apply function to each char of string with index |
| [`ft_putchar_fd`](libft/ft_putchar_fd.c) | Output char to file descriptor |
| [`ft_putstr_fd`](libft/ft_putstr_fd.c) | Output string to file descriptor |
| [`ft_putendl_fd`](libft/ft_putendl_fd.c) | Output string with newline to file descriptor |
| [`ft_putnbr_fd`](libft/ft_putnbr_fd.c) | Output number to file descriptor |

### Bonus Functions (Linked Lists)
| Function | Description |
|----------|-------------|
| [`ft_lstnew`](libft/ft_lstnew_bonus.c) | Create new list node |
| [`ft_lstadd_front`](libft/ft_lstadd_front_bonus.c) | Add node at beginning of list |
| [`ft_lstsize`](libft/ft_lstsize_bonus.c) | Count nodes in list |
| [`ft_lstlast`](libft/ft_lstlast_bonus.c) | Get last node of list |
| [`ft_lstadd_back`](libft/ft_lstadd_back_bonus.c) | Add node at end of list |
| [`ft_lstdelone`](libft/ft_lstdelone_bonus.c) | Delete node with specific deleter |
| [`ft_lstclear`](libft/ft_lstclear_bonus.c) | Delete list with specific deleter |
| [`ft_lstiter`](libft/ft_lstiter_bonus.c) | Apply function to all list nodes |
| [`ft_lstmap`](libft/ft_lstmap_bonus.c) | Create new list by applying function |

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
