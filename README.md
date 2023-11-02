#  C - printf

```` 
int printf ( const char * format, ... );
```

This is a team project work from ALX to create a customized printf

## About the project
This is a rebuild of the standard printf Function in C program. This project is a teamwork as part of our study of C program knowledge in cohort 14 of [ALX Software Engineering Program](https://www.alxafrica.com/software-engineering-2023) that started in the month of April 14th, 2023.

* Prototype: **int _printf(const char *format, ...);**
* General format: **_printf("format string", var1, var2, ...);**

## printf example:
| Data types     |   Std_Input format                |     Std_output     |
|:--------------:|:----------------------------------|:-------------------|
|  String        | _printf("%s\n", 'This is a string.');| This is a string.|
|  character	 | _printf("The first letter in the alphabet is %c\n", 'A');| The first letter in the alphabet is A|
|  Integer	 | _printf("There are %i dozens in a gross\n", 12);| There are 12 dozens in a gross|
|  Decimal	 | _printf("%d\n", 1000);      | 1000|

## Project Requirements
* Allowed editors: **vi**, **vim**, **emacs**
* All files is compiled on **Ubuntu 20.04 LTS using gcc**, using the options **-Wall -Werror -Wextra -pedantic -std=gnu89**
* All files ends with a new line
* There is a **README.md** file, at the root of the folder of the project
* Codes are compiled using the **Betty style**
* The prototypes of all your functions should be included in your header file called **main.h**
* All header files were include guarded
## Authorized functions and macros
* write (man 2 write)
* malloc (man 3 malloc)
* free (man 3 free)
* va_start (man 3 va_start)
* va_end (man 3 va_end)
* va_copy (man 3 va_copy)
* va_arg (man 3 va_arg)

## [Specifier, Flags, Width, Precision, and Length modifiers](https://docs.microsoft.com/en-us/cpp/c-runtime-library/format-specification-syntax-printf-and-wprintf-functions?view=msvc-170)
### Specifier & examples:
|Specifier	 |	Output			     |	     Examples     |
|:--------------:|:----------------------------------|:-------------------|
|c 	         |         Character 	             |     y              |
|d or i         	|Signed integer 	|       1024, -1024|
|s 	      |String of characters                  |    Hello Alx |
|b 	|  Binary Representation of unsigned integer   | 	01010110          |
|u 	|  Unsigned integer 	  |   1024   |
|o 	|  Unsigned octal 	  |   432    |
|x 	|  Unsigned hexadecimal integer  |	3ca   |
|X 	|  Unsigned hexadecimal integer (uppercase)   |  	3CA  |
|S 	|  String with hex-ascii value replacing special chars 	 |     \x0A\x0A   |
|p 	|  Pointer address 	  |        0x403212   |
|r 	|  Reversed string of characters 	|   dlroW olleH    |
|R 	|  ROT13 Translation of string 	  |   Uryyb     |

### Flags (In development...)
|	Flags	 |		Description	      |
|:--------------:|:-----------------------------------|
|- 	|  Left-justify the output within the field width that was given; Right justification is the default (see width sub-specifier). |
|**+** 	|  Preceeds the result with a plus or minus sign **(+ or -)** even for positive numbers. By default, only negative numbers are preceded with a **- sign**. |
|**(space)** |	If no sign is going to be written, a blank space is inserted before the value. |
|**#** 	|  Used with **o**, **x** or **X** specifiers the value is preceeded with **0**, **0x** or **0X** respectively for values different than zero.  |
| **0**     |	Left-pads the number with **zeroes (0)** instead of spaces when padding is specified (see width sub-specifier). |

### Width (In development...)
|	Width	|			Description		|
|:--------------:|:-----------------------------------|
|(number) 	 |Minimum number of characters to be printed. If the value to be printed is shorter than this number, the result is padded with blank spaces. The value is not truncated even if the result is larger. |
|* 	|   The width is not specified in the format string, but as an additional integer value argument preceding the argument that has to be formatted.  |

### Precision (In development...)
|   .Precision   |	Description		      |
|:--------------:|:-----------------------------------|
|**.(number)** 	|  For integer specifiers **(d, i, o, u, x, X)**: precision specifies the minimum number of digits to be written. If the value to be written is shorter than this number, the result is padded with leading zeros. The value is not truncated even if the result is longer. A precision of **0** means that no character is written for the value 0. For **s**: this is the maximum number of characters to be printed. By default all characters are printed until the ending **null** character is encountered. If the period is specified without an explicit value for precision, 0 is assumed.  |

### Length modifiers (In development...)
|   Modifier/Specifier  |  d & i  |  u, o, x, X  |  c   |   s   |   p   |
|:--------------:|:--------:|:-------------:|:---------:|:--------:|:-----------:|
|none 	|  int 	|  unsigned int |  int  |    char pointer  | 	void pointer  |
|h 	|short int | unsigned short int|    |      |     | 			
|l 	|long int  |	unsigned long int   |      |	 |       |

## Mandatory Tasks
- [ ] Write function that produces output with conversion specifiers **c**, **s**, and **%**.
- [ ] Handle conversion specifiers **d**, **i**.
- [ ] Create a man page for your function

## Advanced Tasks  
- [ ] Handle conversion specifier **b**.
- [ ] Handle conversion specifiers **u**, **o**, **x**, **X**.
- [ ] Use a local buffer of 1024 chars in order to call **write** as little as possible.
- [ ] Handle conversion specifier **S**.
- [ ] Handle conversion specifier **p**.
- [ ] Handle flag characters **+**, space, and **#** for non-custom conversion specifiers.
- [ ] Handle length modifiers **l** and **h** for non-custom conversion specifiers.
- [ ] Handle the field width for non-custom conversion specifiers.
- [ ] Handle the precision for non-custom conversion specifiers.
- [ ] Handle the **0** flag character for non-custom conversion specifiers.
- [ ] Handle the custom conversion specifier **r** that prints the reversed string.
- [ ] Handle the custom conversion specifier **R** that prints the rot13'ed string.
- [ ] All above options should work well together.

## List of files and description:
| S/N   |       files          |        Description  |
|:-----:|:--------------------:|:--------------------|
|  1.   |		       |		     |


## [Flowchart.](https://photos.app.goo.gl/5SQMnxrmd7nkLr3a6)
## How to use.
### Complilation 
All of the ``.c`` files along with a main.c file are to be compiled with ``gcc 4.8.4`` on Ubuntu 14.04 LTS with the flags ``-Wall Werror`` ``-Westra`` and ``-pedantic.``

The files will be compiled this way:
- ``gcc -Wall -Werror -Wextra -pedantic *.c````

## Authors
- [Oladimei Olayinka](https://github.com/holladworld)  
- [ILESANMI Esther](https://github.com/Ilesanmiester)


## Acknowledgement
This is an open source test project in line with Requirements from [ALX](https://alxafrica.com)

