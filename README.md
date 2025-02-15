# Libft

## Introduction

The **Libft** project at 42 is designed to introduce students to the concept of building their own C standard library. This project requires implementing a set of essential functions from ```<string.h>```, ```<stdlib.h>```, and other standard C libraries, allowing students to gain a deep understanding of memory management, string manipulation, and linked list operations.

## Concept

Libft is a foundational project that challenges students to write and optimize their own versions of common C library functions. The goal is to create a reusable library that can be used in future projects at 42.

The project covers:

  - **Memory manipulation functions** (e.g., ```memset```, ```bzero```, ```memcpy```, ```memmove```, ```calloc```, ```realloc```)

  - **String manipulation functions** (e.g., ```strlen```, ```strdup```, ```strjoin```, ```strtrim```)

  - **Character classification functions** (e.g., ```isdigit```, ```isalpha```, ```toupper```, ```tolower```)

  - **Linked list operations** (e.g., ```lstnew```, ```lstadd_front```, ```lstadd_back```, ```lstsize```, ```lstdelone```)

## Mandatory Requirements

  - Implement a static library called ```libft.a``` containing the required functions.

  - Functions must match their standard library counterparts in behavior and return values.

  - Memory allocation functions must properly handle errors.

  - Implement additional utility functions to extend the library’s functionality.

  - No use of external libraries or unauthorized functions.

## Bonus Features

  - Implement additional linked list functions such as:

    - ```ft_lstmap()``` - Applies a function to each node of a linked list.

    - ```ft_lstiter()``` - Iterates through a linked list.

  - Implement functions to handle more complex string operations.

## Implementation Details

### Memory Manipulation Functions

  - ```ft_memset(void *s, int c, size_t n)```: Fills ```n``` bytes of memory with the specified byte c.

  - ```ft_bzero(void *s, size_t n)```: Sets ```n``` bytes of memory to zero.

  - ```ft_memcpy(void *dest, const void *src, size_t n)```: Copies ```n``` bytes from src to dest.

  - ```ft_memmove(void *dest, const void *src, size_t n)```: Copies ```n``` bytes, handling overlapping memory regions.

### String Manipulation Functions

  - ```ft_strlen(const char *s)```: Returns the length of a string.

  - ```ft_strcpy(char *dest, const char *src)```: Copies ```src``` into ```dest```.

  - ```ft_strcat(char *dest, const char *src)```: Appends ```src``` to ```dest```.

  - ```ft_strjoin(const char *s1, const char *s2)```: Concatenates two strings and returns a new string.

### Character Classification Functions

  - ```ft_isalpha(int c)```: Checks if a character is an alphabetic letter.

  - ```ft_isdigit(int c)```: Checks if a character is a digit.

  - ```ft_isalnum(int c)```: Checks if a character is alphanumeric.

  - ```ft_tolower(int c)```: Converts an uppercase letter to lowercase.

  - ```ft_toupper(int c)```: Converts a lowercase letter to uppercase.

### Linked List Functions

  - ```ft_lstnew(void *content)```: Creates a new list node with the given content.

  - ```ft_lstadd_front(t_list **lst, t_list *new)```: Adds a new node at the beginning of the list.

  - ```ft_lstadd_back(t_list **lst, t_list *new)```: Adds a new node at the end of the list.

  - ```ft_lstsize(t_list *lst)```: Returns the number of nodes in a list.

  - ```ft_lstclear(t_list **lst, void (*del)(void *))```: Deletes and frees the entire list.

## Compilation and Usage

To use ```libft.a``` in another project, include the header file:

```c
#include "libft.h"
```

To compile the library, run:

```console
make
```

To clean object files:

```console
make clean
```

To remove all compiled files:

```console
make fclean
```

To recompile everything:

```console
make re
```

## Common Pitfalls

$\color{crimson}{\textbf{Memory Leaks}}$: Always ensure that dynamically allocated memory is properly freed.

$\color{crimson}{\textbf{Undefined Behavior}}$: Pay attention to buffer overflows and null pointer dereferencing.

$\color{crimson}{\textbf{Function Matching}}$: Make sure each function behaves exactly like its standard library equivalent.

$\color{crimson}{\textbf{Makefile Errors}}$: Ensure that ```make clean```, ```make fclean```, and ```make re``` work correctly.

## Conclusion

The $\color{RoyalBlue}{\textbf{Libft}}$ project is a foundational part of the 42 curriculum, helping students develop a deeper understanding of C programming, memory management, and efficient algorithm implementation. Mastering this project is crucial, as the functions implemented here will be reused in many future projects.
