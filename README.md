# MY_LIBRARY

## Table of Contents
- [About](#about)
- [Compilation](#compilation)
- [Key Concepts Learned](#key-concepts-learned)
- [Skills Developed](#skills-developed)
- [Modules Overview](#modules-overview)
- [42 School Standards](#42-school-standards)
- [Related Articles](#-related-articles)
- [Contact](#contact)


## About

This repository contains my unified personal C library, bundling three foundational 42 School projects: **libft**, **get_next_line**, and **ft_printf**. It serves as the base toolbox reused across virtually every other 42 project.

Together, these modules build a solid understanding of C programming, pointers, memory management, string manipulation, file descriptor I/O, and variadic functions.


## Compilation

A single Makefile builds the whole library:

```bash
# Compile the library (produces libft.a)
make

# Clean object files
make clean

# Clean everything (including libft.a)
make fclean

# Recompile from scratch
make re
```

Include in your projects with:
```c
#include "my_library.h"
```


## Key Concepts Learned

### Fundamental C Programming
- **Pointers and Memory**: Mastery of pointer manipulation and dynamic memory allocation
- **String Manipulation**: Building and handling strings at a low level
- **Data Structures**: Implementing linked lists and managing nodes
- **Function Pointers**: Using callbacks for flexible function design

### Library Development
- **Modular Code**: Creating reusable and self-contained functions
- **Header and Source Separation**: Organizing code for clarity and maintainability
- **Error Handling**: Defensive programming and consistent return values
- **Code Norm Compliance**: Adhering to 42's coding standards and style guides

### Core C Concepts
- **Memory Management**: Manual allocation, deallocation, and avoiding leaks
- **Variadic Functions**: Implementing functions with a variable number of arguments (printf)
- **Static Buffers**: Persisting state across calls (get_next_line)
- **Static vs Dynamic Linking**: Basics of library creation and usage
- **Function Reimplementation**: Deep understanding through re-coding standard libc functions


## Skills Developed

- **C Language Proficiency**: Solid grasp of C syntax and semantics
- **Low-level Programming**: Effective use of pointers, memory, and system calls
- **Library Creation**: Building a foundational C library with useful utilities
- **Problem Solving**: Tackling edge cases and implementing robust algorithms
- **Code Quality & Style**: Writing clean, readable, and norm-compliant code
- **Debugging and Testing**: Validating function correctness and memory safety


## Modules Overview

### `libft/` — Standard library reimplementation
Reimplementations of common libc functions and utility helpers:
- Character and string manipulation (`ft_strlen`, `ft_strchr`, `ft_strncmp`, `ft_split`, `ft_substr`, `ft_strjoin`, ...)
- Memory management (`ft_memset`, `ft_memcpy`, `ft_calloc`, `ft_bzero`, ...)
- Conversion and checks (`ft_atoi`, `ft_itoa`, `ft_isalpha`, `ft_isdigit`, ...)
- Linked lists (`ft_lstnew`, `ft_lstadd_back`, `ft_lstmap`, `ft_lstclear`, ...)
- Output to file descriptors (`ft_putchar_fd`, `ft_putstr_fd`, `ft_putnbr_fd`, ...)

### `get_next_line/` — Read a file line by line
Reads from a file descriptor one line at a time, regardless of the buffer size, using a static variable to persist leftover data between calls. Supports multiple file descriptors simultaneously.

### `printf/` — Custom printf implementation
A reimplementation of `printf` covering the most common format specifiers (`%c`, `%s`, `%p`, `%d`, `%i`, `%u`, `%x`, `%X`, `%%`), built on top of variadic functions (`va_list`, `va_start`, `va_arg`, `va_end`).

This unified library is reused across every other 42 project that requires foundational C utilities.


## 42 School Standards

### Norm Requirements
- ✅ Maximum 25 lines per function
- ✅ Maximum 5 functions per file
- ✅ Proper indentation and formatting
- ✅ No forbidden functions usage
- ✅ Compilation without warnings

### Coding Standards
- ✅ No memory leaks (checked with valgrind)
- ✅ Robust handling of edge cases (NULL, empty input, large inputs)
- ✅ Consistent return values matching the libc reference
- ✅ Reusable, self-contained modular functions


## 📝 Related Articles

Blog posts documenting the learning process and context behind this project:

- 📝 [42 Piscine and Common Core: What I Learned](https://arthur-portfolio.com/en/blog/42-piscine-and-core-curriculum) — Reflections on 42 School's selection process and 2-year curriculum

---
## Contact

- **GitHub**: [@TuroTheReal](https://github.com/TuroTheReal)
- **Email**: arthurbernard.dev@gmail.com
- **LinkedIn**: [Arthur Bernard](https://www.linkedin.com/in/arthurbernard92/)

---

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-C-blue.svg"/>
</p>
