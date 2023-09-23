# Project: 0x11. C - printf

## Resources

#### Read or watch:

* [Secrets of printf](https://intranet.alxswe.com/rltoken/7Vw7aUWgwC7JYUrqI4bh4Q)
* [Group Projects concept page (Don’t forget to read this)]()
* [Flowcharts concept page]()
## Tasks

| Task | File |
| ---- | ---- |
| 0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life | [SOON](./) |
| 1. Education is when you read the fine print. Experience is what you get if you don't | [SOON](./) |
| 2. With a face like mine, I do better in print | [SOON](./) |
| 3. What one has not experienced, one will never understand in print | [SOON](./) |
| 4. Nothing in fine print is ever good news | [SOON](./) |
| 5. My weakness is wearing too much leopard print | [SOON](./) |
| 6. How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print | [SOON](./) |
| 7. The big print gives and the small print takes away | [SOON](./) |
| 8. Sarcasm is lost in print | [SOON](./) |
| 9. Print some money and give it to us for the rain forests | [SOON](./) |
| 10. The negative is the equivalent of the composer's score, and the print the performance | [SOON](./) |
| 11. It's depressing when you're still around and your albums are out of print | [SOON](./) |
| 12. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection | [SOON](./) |
| 13. Print is the sharpest and the strongest weapon of our party | [SOON](./) |
| 14. The flood of print has turned reading into a process of gulping rather than savoring | [SOON](./) |
| 15. * | [SOON](./) |

# More Info
Authorized functions and macros
write (man 2 write)
malloc (man 3 malloc)
free (man 3 free)
va_start (man 3 va_start)
va_end (man 3 va_end)
va_copy (man 3 va_copy)
va_arg (man 3 va_arg)

Compilation
Code will be compiled this way:
$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c

# Tasks

0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life

Write a function that produces output according to a format.

Prototype: int _printf(const char *format, ...);
Returns: the number of characters printed (excluding the null byte used to end output to strings)
write output to stdout, the standard output stream
format is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. You need to handle the following conversion specifiers:
c
s
%
You don’t have to reproduce the buffer handling of the C library printf function
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers

    
1. Education is when you read the fine print. Experience is what you get if you don't

Handle the following conversion specifiers:

d
i
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers

    
2. With a face like mine, I do better in print
#adv
Handle the following custom conversion specifiers:

b: the unsigned int argument is converted to binary
alex@ubuntu:~/c/printf$ cat main.c
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%b\n", 98);
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
alex@ubuntu:~/c/printf$ ./a.out
1100010
alex@ubuntu:~/c/printf$

   
3. What one has not experienced, one will never understand in print
#adv
Handle the following conversion specifiers:

u
o
x
X
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers

    
4. Nothing in fine print is ever good news
#adv
Use a local buffer of 1024 chars in order to call write as little as possible.

    
5. My weakness is wearing too much leopard print
#adv
Handle the following custom conversion specifier:

S : prints the string.
Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)
alex@ubuntu:~/c/printf$ cat main.c
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%S\n", "Best\nSchool");
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
alex@ubuntu:~/c/printf$ ./a.out
Best\x0ASchool
alex@ubuntu:~/c/printf$

   
6. How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print
#adv
Handle the following conversion specifier: p.

You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers

    
7. The big print gives and the small print takes away
#adv
Handle the following flag characters for non-custom conversion specifiers:

+
space
#

    
8. Sarcasm is lost in print
#adv
Handle the following length modifiers for non-custom conversion specifiers:

l
h
Conversion specifiers to handle: d, i, u, o, x, X

    
9. Print some money and give it to us for the rain forests
#adv
Handle the field width for non-custom conversion specifiers.

    
10. The negative is the equivalent of the composer's score, and the print the performance
#adv
Handle the precision for non-custom conversion specifiers.

     
11. It's depressing when you're still around and your albums are out of print
#adv
Handle the 0 flag character for non-custom conversion specifiers.

    
12. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection
#adv
Handle the - flag character for non-custom conversion specifiers.

    
13. Print is the sharpest and the strongest weapon of our party
#adv
Handle the following custom conversion specifier:

r : prints the reversed string
    
14. The flood of print has turned reading into a process of gulping rather than savoring
#adv
Handle the following custom conversion specifier:

R: prints the rot13'ed string
    
15. *
#adv
All the above options work well together.


Contributors:

Perpetual Okorie [AmazedWonder](https://github.com/AmazedWonder)

Tsitsi-del [Tsitsi-del](https://github.com/Tsitsi-del)
