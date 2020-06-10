Structure of a C program

We are about to enter the most interesting, the programming itself; but it is necessary, first; mention some of the typical errors when programming, so that the reader knows how to identify them and can correct them.

SYNTAX ERROR: These errors are produced when the rules of the programming language are misused, and the syntax rules of that language are violated (in our case C); These errors are easy to detect because it is generally the compiler that identifies them (and even shows the line where the error is found, but that depends on the version of the compiler we are using). In this course I have used Turbo C, in version 2 and 3.
IMPLEMENTATION ERRORS: These errors occur when we tell the computer to perform a certain action, and it understands it, but cannot execute it. For example, tell the computer a division by zero, add two variables to which no value has been assigned, etc.
LOGIC ERRORS: Many times, when we are programming, the compiler does not indicate syntax or logic errors; but the result of our program is out of the expected range, this is the product of a logic error in the code of our program. These types of errors are very difficult to identify and, of course, to correct, since we generally have to review our program line by line. Example: The negative salary of an employee, etc.
The structure of a C program consists of some essential parts: which are one or more modules called functions, with main () being the first function that is called when the program execution begins.

Each function must contain:

> Pre-processor directives (instructions given to the compiler

#include before compiling)

#define

example:

#include <stdio.h>

What you are being told is that of the libraries, "Include" in our program the directive stdio.h, which contains the functions of input and output of data (standard input output, in English). If we need the mathematical functions, we must specify it with the declaration:

#include <math.h>

If we need the string functions:

#inlcude <stlib.h>

It is necessary to clarify that this is done at the beginning of the program, and the declarations must have the numeral symbol (#) followed by the "include" statement, and between greater and less than (<>) the name of the directive.

> Global Declarations

They may be:

* Function Prototypes: Also called function declarations, which will be discussed later

* Variable Declarations

It should be noted that this is done followed by #include and #define.

> Main function main ()

This is the main function of our program, your body, so it should NEVER be missing, since all the instructions of our program are contained in it.

main ()

{

local statements / * Comments * /

sentences

}

the main () function goes to the beginning, then we open curly brackets and within them go the variable declarations, the reading statements, calculations, assignments and impressions, and with the last brace (}), we indicate the end of the program.

Example 1.1

Program that calculates the area of ​​a circle from the radius

#include <stdio.h>

#include <conio.h>

main ()

{

float radio, area;

printf ("Radius = \ n");

scanf ("% f", & radio);

area = 3.14159 * radio * radio;

printf ("The Area is% f \ n \ n", area);

getch ();

return 0;

}

Explanation:

We told the compiler that we will use the <stdio.h> and <conio.h> libraries, why <conio.h> ?, because this library contains the functions getche (), getch (), etc, and we use one of them in this small example.

Then, we indicate to our program the beginning of our program (function main ()).

We declare, as real values, the variables radius and area (this will be discussed later). Then, with the printf () instruction, we display the message (Radio =) on the screen and scanf takes care of reading the value entered by the user. Subsequently area, is equal to the multiplication of pi (3.14159), the radius squared. That result is shown on the screen, then the program waits for any key to be pressed (getch ()) and does not return any value (return 0).

Credits:
Luisa Arboleda