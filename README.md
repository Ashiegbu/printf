Alx paired team project
printf()
The printf project is a collaboration between Kingsley Emeka Umunna and Chibuzo Ashiegbu, actual students of Software Engineering at ALX Software Engineering Progromme , were a function named "_printf" imitates the actual "printf" command located in the stdio.h library. It contains some of the basic features and functions found in the manual 3 of "printf".

_printf() is a function that performs formatted output conversion and print data. Its prototype is the following:

int _printf(const char *format, ...)
Where format contains the string that is printed. As _printf() is variadic function, it can receives n arguments that replace by n tags written inside the string.

The format tags prototype is the following:

%[flags][length]specifier
If the program runs successfully, the return value is the amount of chars printed.

Specifier	Output
c	Character
d or i	Signed decimal integer
s	String of characters
b	Signed binary
o	Signed octal
u	Unsigned integer
x	Unsigned hexadecimal
X	Unsigned hexadecimal (uppercase)
p	Pointer address
r	Reverse string of characters
R	ROT13 translation of string
S	String with special chars replaced by their ASCII value
%	Character
Flags	Description	Specifiers
+	Prints a plus sign (+) when the argument is a positive number. In other case, prints a minus sign (-).	i, d
(space)	Prints a blank space if the argument is a positive number	i, d
#	Prints 0, 0x and 0X for o, x and X specifiers, respectively. It doesn't print anything if the argument is zero	o, x, X
Length	Description	Specifiers
l	Prints a long int or unsigned long int	i, d, o, u, x and X
h	Prints a short int or unsigned short int	i, d, o, u, x and X
Examples
Printing the string of chars "Hello,ALX ":

Use: _printf("Hello ALX%s.", "ALX");
Output: Hello ALX .
Printing an integer number:

Use: _printf("10 + 10 is equal to %d.", 20);
Output: 10 + 10 is equal to 20.
Printing a binary, octal and hexadecimal:

Use: _printf("10 in binary is [%b], in octal is [%o] and in hexadecimal is [%x]", 5, 5, 5);
Output: 10 in binary is [1010], in octal is [12] and in hexadecimal is [A]
Printing a string codified in ROT13:

Use: _printf("Hello in ROT13 is %R", "Hello");
Output: Hello in ROT13 is Urybb
Using flags and length tags:

Printing the string of chars "Hello, ALX ":

Use: _printf("2 * 2 = %+d and 5 * -5 = %+i", 4, -25);
Output: 2 * 2 = +4 and 5 * -5 = -25
Printing a long integer number and short integer number:

Use: _printf("1 million as a long int is %ld, but as a short int is %hd", 1000000, 1000000);
Output: 1 million as a long int is 1000000, but as a short int is 16960
File Functions
main.h
