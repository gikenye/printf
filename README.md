
# _printf
---
```_printf```

**Prototype:** ```int _printf(const char *, ...);```

## Examples
**String**
* Input: ```_printf("%s\n", 'This is a string.');```
* Output: ```This is a string.```

**Character**
* Input: ```_printf("The first letter in the alphabet is %c\n", 'A');```
* Output: ```The first letter in the alphabet is A```

**Integer**
* Input: ```_printf("There are %i dozens in a gross\n", 12);```
* Output: ```There are 12 dozens in a gross```

**Decimal:**
* Input: ```_printf("%d\n", 1000);```
* Output:  ```1000```
## Project Requirements
* All files will be compiled on Ubuntu 14.04 LTS
* Programs and functions will be compiled with gcc 4.8.4 using flags -Wall -Werror -Wextra and -pedantic
* Code must follow the [Betty](https://github.com/holbertonschool/Betty/wiki) style
* Global variables are not allowed
* Authorized functions and macros:
  * ```write``` (man 2 write)
  * ```malloc``` (man 3 malloc)
  * ```free``` (man 3 free)
  * ```va_start``` (man 3 va_start)
  * ```va_end``` (man 3 va_end)
  * ```va_copy``` (man 3 va_copy)
  * ```va_arg``` (man 3 va_arg)
## Mandatory Tasks
- [x] Write function that produces output with conversion specifiers ```c```, ```s```, and ```%```.
- [x] Handle conversion specifiers ```d```, ```i```.
- [x] Create a man page for your function.
## Advanced Tasks
- [x] Handle conversion specifier ```b```.
- [x] Handle conversion specifiers ```u```, ```o```, ```x```, ```X```.
- [ ] Use a local buffer of 1024 chars in order to call write as little as possible.
- [x] Handle conversion specifier ```S```.
- [x] Handle conversion specifier ```p```.
- [ ] Handle flag characters ```+```, space, and ```#``` for non-custom conversion specifiers.
- [ ] Handle length modifiers ```l``` and ```h``` for non-custom conversion specifiers.
- [ ] Handle the field width for non-custom conversion specifiers.
- [ ] Handle the precision for non-custom conversion specifiers.
- [ ] Handle the ```0``` flag character for non-custom conversion specifiers.
- [x] Handle the custom conversion specifier ```r``` that prints the reversed string.
- [x] Handle the custom conversion specifier ```R``` that prints the rot13'ed string.
- [ ] All above options should work well together.
## File Descriptions
* **_printf.c:** - contains the  fucntion ```_printf```, which uses the prototype ```int _printf(const char *format, ...);```. The format string is composed of zero or more directives. See ```man 3 printf``` for more detail. **_printf** will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to **stdout**, the standard output stream.
* **_putchar.c:** - contains the function ```_putchar```, which writes a character to stdout.
* **holberton.h:** - contains all function prototypes used for ```_printf```.
* **man_3_printf:** - manual page for the custom ```_printf``` function.
* **print_chars.c:** - contains the functions ```print_c```, ```print_s```, ```print_S```, and ```print_r``` which handle the conversion specifiers ```c```, ```s```, ```S```, and ```r```, respectively, as well as ```hex_print```, which prints a char's ascii value in uppercase hex
* **print_numbers.c:** - contains the functions ```print_i``` and ```print_d```, which handle the conversion specifiers ```i``` and ```d```, respectively
* **print_hex.c:** - contains the functions ```print_hex```, which prints an unsigned int in hexidecimal form, ```print_x```, ```print_X```, and ```print_p```, which handle the conversion specifiers ```x```, ```X```, and ```p```, respectively
* **print_unsigned_int.c:** - contains the functions ```print_u```, ```print_o```, and ```print_b```, which handle the conversion specifiers ```u```, ```o```, and ```b```, respectively
* **print_rot13.c** - contains the function ```print_R```, which handles the conversion specifier ```R```
## Authors
[Johnstone Njuguna](https://github.com/gikenye) 
[Omondi Jeff](https://github.com/kojeffi) 
```
---# printf
