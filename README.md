# LIBFT – 42 School C Standard Library

This project is a personal implementation of common C standard library functions, developed as part of the 42 school curriculum. It includes essential memory and string operations, character checks, and linked list utilities.

This version passed all mandatory and bonus requirements.

## 📁 Project Structure

All source and header files are located in the root directory.


## ✅ Features

### Mandatory Part

- `memcpy`, `memset`, `bzero`, `memmove`, `memcmp`, `memchr`
- `strlen`, `strlcpy`, `strlcat`, `strchr`, `strrchr`, `strncmp`, `strnstr`
- `atoi`, `calloc`, `strdup`
- `isalpha`, `isdigit`, `isalnum`, `isascii`, `isprint`, `toupper`, `tolower`
- `putchar_fd`, `putstr_fd`, `putendl_fd`, `putnbr_fd`
- `strjoin`, `strtrim`, `split`, `itoa`, `substr`, `strmapi`, `striteri`

### Bonus Part

- Singly linked list (`t_list`) utilities:
  - `lstnew`, `lstadd_front`, `lstsize`, `lstlast`, `lstadd_back`
  - `lstdelone`, `lstclear`, `lstiter`, `lstmap`

## 🛠️ Build Instructions

Run the following command in the project directory:

```bash
make
```

Compiles only the mandatory part of the library.
Creates the static library file libft.a.

```bash
make bonus
```

Compiles both the mandatory and bonus functions (e.g., linked list utilities).
Also produces libft.a with all symbols included.

```bash
make clean      # Removes object files
make fclean     # Removes object files and libft.a
make re         # Runs fclean and then make
```

## 🧪 Usage Example
```c
#include "libft.h"

int main(void)
{
    char *s = ft_strdup("Hello, world!");
    ft_putendl_fd(s, 1);
    free(s);
    return 0;
}
```
Compile with:
```bash
gcc main.c -L. -lft
```
💡 Note: This command is for testing libft.a in your own programs. The library itself must be compiled using make or make bonus as required by the 42 school project rules.

## 👤 Author

[Martin Justa](https://github.com/aztaban)