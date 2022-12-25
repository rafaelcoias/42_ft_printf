# 42_ft_printf
### Assignment

This project is about programming the famous printf() function.

### Skills Learned

  - Rigor
  - Algorithms & AI

<h3>Goal</h3>

The goal of this project is pretty straightforward. You will recode printf().
You will mainly learn about using a variable number of arguments.
Finally, you can add this function to your own library.

<h3>What you need to know before starting ft_printf</h3>
<h4>Varying number of arguments</h4> 
You will learn about <i>va_list</i> arguments. It is used when a function receives a varying amount of arguments like printf : <br>
int ft_printf(char *str, <b>...<b/>) <br>
The '...' means that this function receives a varying amount of arguments (of varying types).

<h4>#include &#60;stdarg&#62;</h4>
  
You are going to need 3 functions to do ft_printf : va_start(), va_arg() and va_end(). <br>
The called function must declare an object of type va_list which is used by the macros va_start(), va_arg(), and va_end().

-  The va_start() macro initializes ap for subsequent use by va_arg() and va_end(), and must be called first. va_starts() basically starts the use of <i>va_list</i>. 

-  The va_arg() macro expands to an expression that has the type and value of the next argument in the call. The argument ap is the va_list ap initialized by va_start(). Each call to va_arg() modifies ap so that the next call returns the next argument.
  
-   Each invocation of va_start() must be matched by a corresponding invocation of va_end() in the same function. After the call va_end(ap) the variable ap is undefined. va_end() basically ends the use of <i>va_list</i>. 

  Learn more here : <a href="https://linux.die.net/man/3/stdarg">man stdarg</a> <br>
  See some examples here : <a href="https://www.thinkage.ca/gcos/expl/c/incl/stdarg.html">va_list example 1</a> and <a href="https://www.includehelp.com/c-programs/va_start-and-va_end-functions-of-stdarg-h-in-c.aspx">va_list example 2</a>

<h4>Flag checking</h4>

It is important that you know printf flags. You are going to need a function to check what flag did the user use.
  - %c Prints a single character
  - %s Prints a string (as defined by the common C convention).
  - %p The void * pointer argument has to be printed in hexadecimal format.
  - %d Prints a decimal (base 10) number.
  - %i Prints an integer in base 10.
  - %u Prints an unsigned decimal (base 10) number.
  - %x Prints a number in hexadecimal (base 16) lowercase format.
  - %X Prints a number in hexadecimal (base 16) uppercase format.
  - %% Prints a percent sign.

Learn more here : <a href="https://man7.org/linux/man-pages/man3/printf.3.html">man printf</a>

<h4>Do not forget</h4>

Printf always returns an integer, so ft_printf must do it too. It is important that you don't forget this once you started the project.

<details><summary>My grade</summary>
  
  ![image](https://user-images.githubusercontent.com/91686183/169927289-9e8dcfa1-7789-4b1d-a6fb-b9d1b8f90dce.png)
  
</details> 
 
<hr>
I hope you found it interesting! <br>
And if you are going to do ft_printf, I wish you good luck and hope that you learned something here!
