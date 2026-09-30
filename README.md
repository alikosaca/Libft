# Libft

My own implementation of a subset of the C standard library, plus extra string and linked-list utilities. This is the first project of the 42 Common Core; the library is reused in almost every later C project.

## What's inside

**libc re-implementations**

| Category | Functions |
|---|---|
| Character checks | `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`, `ft_toupper`, `ft_tolower` |
| Memory | `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`, `ft_memchr`, `ft_memcmp`, `ft_calloc` |
| Strings | `ft_strlen`, `ft_strlcpy`, `ft_strlcat`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`, `ft_strnstr`, `ft_strdup`, `ft_atoi` |

**Additional functions**

`ft_substr`, `ft_strjoin`, `ft_strtrim`, `ft_split`, `ft_itoa`, `ft_strmapi`, `ft_striteri`, `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`

**Linked list (bonus)**

`ft_lstnew`, `ft_lstadd_front`, `ft_lstadd_back`, `ft_lstsize`, `ft_lstlast`, `ft_lstdelone`, `ft_lstclear`, `ft_lstiter`, `ft_lstmap`

## Usage

```bash
make          # builds libft.a
make bonus    # adds the linked-list functions
```

Link it into your project:

```bash
cc -Wall -Wextra -Werror main.c -L. -lft -o app
```

## What I learned

- Manual memory management with `malloc` / `free` and avoiding leaks
- Handling overlapping memory (`memmove` vs `memcpy`)
- Pointer arithmetic and building a reusable static library with a Makefile

## License

MIT
