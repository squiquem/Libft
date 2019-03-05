# Libft

First 42-school project : recoding a 'libft.a' library, identical to libc for the first part and following instructions for the second.
____

## Part 1  

Check 'man' for the description of the following functions :
- ft_memset
- ft_bzero  
- ft_memcpy
- ft_memccpy
- ft_memmove
- ft_memchr
- ft_memcmp
- ft_strlen
- ft_strdup
- ft_strcpy
- ft_strncpy
- ft_strcat
- ft_strncat
- ft_strlcat
- ft_strchr
- ft_strrchr
- ft_strstrs
- ft_strnstr
- ft_strcmp
- ft_strncmp
- ft_atoi
- ft_isalpha
- ft_isdigit
- ft_isalnum
- ft_isascii
- ft_isprint
- ft_toupper
- ft_tolower
____

## Part 2

#### ft_memalloc
> Allocates memory with 'malloc(3)' and returns a fresh memory area. Allocated memory is initialied to 0. If allocating fails, returns 'NULL'

#### ft_memdel
> Takes as parameter a pointer address which pointed area has to be freed with 'free(3)', then the pointer becomes 'NULL'

#### ft_strnew
> Allocates memory with 'malloc(3)' and returns a new string ended with '\0'. Every char is initialized to '\0'; if allocating fails, returns 'NULL'

#### ft_strdel
> Takes as parameter a string address which has to be freed with 'free(3)' and its pointer put to 'NULL'

#### ft_strclr
> Assigns '\0' to every char of the string in parameter

#### ft_striter
> Applies the function 'f' to every char of the string in parameter. Every char is taken by address to the 'f' in order to be modified if necessary

#### ft_striteri
> Applies the function 'f' to every char of the string in parameter, precising its index as first argument. Every char is taken by address to 'f' in order to be modified if necessary

#### ft_strmap
> Applies the function 'f' to every char of the string in parameter to create a new string with 'malloc(3)' coming from successive applications of 'f'

#### ft_strmapi
> Applies the function 'f' to every char of the string in parameter precising its index to create a new string with 'malloc(3)'coming from successive applications of 'f'

#### ft_strequ
> Compares lexicographically strings 's1' and 's2'. If equal, function returns 1, else 0

#### ft_strnequ
> Compares lexicographically strings 's1' and 's2' until n char max, or until meeting '\0'. If equal, functions returns 1, else 0

#### ft_strsub
> Allocates memory with 'malloc(3)' and returns new copy of a section of the string in parameter. The section starts at index 'start' and its length is 'len'. If 'start' and 'len' don't show a valid section, attitude is undetermined. If allocation fails, returns 'NULL'

#### ft_strjoin
> Allocates memory with 'malloc(3)' and returns a new string ended by '\0' resulting from the concatenation of strings 's1' and 's2'. If allocating fails, returns 'NULL'

#### ft_strtrim
> Allocates memory with 'malloc(3)' and returns a copy of the string in parameter without the blank spaces at start and at end. Blank spaces are ' ', '\n' and '\t'. If 's' has no blank spaces at start or at end, function returns a copy of 's'. If allocating fails, returns 'NULL'

#### ft_strsplit
> Allocates memory with 'malloc(3)' and returns a table of new strings (all ended by '\0', so is the table) resulting from the section of string 's' according to char 'c'. If allocating fails, returns 'NULL'

#### ft_itoa
> Allocates memory with 'malloc(3)' and returns a new string ended by '\0' showing the int 'n' in parameter. Negative numbers are managed. If allocating fails, returns 'NULL'

#### ft_putchar
> Displays char 'c' on standard output

#### ft_putstr
> Displays string 's' on standard output

#### ft_putendl
> Displays string 's' followed by '\n' on standard output

#### ft_putnbr
> Displays int 'n' on standard output

#### ft_putchar_fd
> Displays char 'c' on file descriptor 'fd'

#### ft_putstr_fd
> Displays string 's' on file descriptor 'fd'

#### ft_putendl_fd
> Displays string 's' followed by '\n' on file descriptor 'fd'

#### ft_putnbr_fd
> Displays int 'n' on file descriptor 'fd'
____

## Bonus part

#### ft_lstnew
> Allocates memory wih 'malloc(3)' and returns a new link. The new link fields 'content' and 'content_size' are initialized by function parameters copy; ff parameter 'content' is null, fields 'content' and 'content_size' are initialized to 'NULL' and '0' even if 'content_size' parameter isn't null; 'next' field is initialized to 'NULL'; if allocating fails, returns 'NULL'

#### ft_lstdelone
> Takes as parameter a pointer address to a link and frees the content memory with function 'del' in parameter, then frees the link memory with 'free(3)'; 'next' field memory must not be freed; pointer to freed link must be set to 'NULL' (like ft_memdel)

#### ft_lstdel
> Takes in parameter a pointer address to a link and frees the memory of this link and of all its followers with function 'del' and 'free(3)'; Pointer to the first freed link must be set to 'NULL' (like ft_memdel)

#### ft_lstadd
> Adds the 'new' element at the beginning of the list

#### ft_lstiter
> Goes through 'lst' list and applies function 'f' to every link

#### ft_lstmap
> Goes through 'lst' list, applies function 'f' to every link and creates a new list allocated with 'malloc(3)' resulting from the successive applications;  if allocating fails, returns 'NULL'
____

## Personal bonus part

### ft_strrev
> Returns the reversed string in parameter

### ft_swap
> Swaps 2 int values

### ft_sqrt
> Calculates the closest int to the square root of the parameter

### ft_whitespace
> Returns 1 if the char 'c' is ' ', '\t', '\n', '\v', '\f' or '\r', else 0

### ft_is_prime
> Returns 1 if the parameter is a prime number
