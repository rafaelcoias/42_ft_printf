# 42_ft_printf
<h3>Assignment</h3>

This project is about programming the famous printf() function.

<h3>Goal</h3>

The goal of this project is pretty straightforward. You will recode printf().
You will mainly learn about using a variable number of arguments.
Finally, you can add this function to your own library.

<h3>What you need to know before starting ft_printf</h3>
<h4>Varying number of arguments</h4> 
You will learn about <i>va_list</i> arguments. It is used when a function receives a varying amount of arguments like printf : <br>
int ft_printf(char *str, <b>...<b/>) <br>
The '...' means that this function receives a varying amount of arguments (of varying types).

You are going to need 3 functions to do ft_printf : va_start(), va_arg() and va_end(). <br>
The called function must declare an object of type va_list which is used by the macros va_start(), va_arg(), and va_end().

-  The va_start() macro initializes ap for subsequent use by va_arg() and va_end(), and must be called first.

-  The va_arg() macro expands to an expression that has the type and value of the next argument in the call. The argument ap is the va_list ap initialized by va_start(). Each call to va_arg() modifies ap so that the next call returns the next argument.
  
-   Each invocation of va_start() must be matched by a corresponding invocation of va_end() in the same function. After the call va_end(ap) the variable ap is undefined.

Learn more here : <a href="https://en.wikipedia.org/wiki/Static_variable">static variables Wikipedia</a> and <a href="https://www.geeksforgeeks.org/static-variables-in-c/">static variables Geeks4Geeks</a>

<h4>Read function</h4>

Read() - read from a file descriptor <br>
The function read() attempts to read up to <i>count</i> bytes from file descriptor <i>fd</i> into the buffer starting at <i>buf</i>. <br>
read(int <b>fd</b>, void <b>*buf</b>, size_t <b>count</b>); <br>

Learn more here : <a href="https://man7.org/linux/man-pages/man2/read.2.html">man read</a>

<h4>Malloc and Free</h4>

Long story short, malloc() is used to allocate memory.
- The malloc() function allocates size bytes and returns a pointer
       to the allocated memory.  The memory is not initialized.  If size
       is 0, then malloc() returns either NULL, or a unique pointer
       value that can later be successfully passed to free().
       
Long story short, free() is used to free the memory space pointed by the pointer.
- The malloc() function allocates size bytes and returns a pointer
       to the allocated memory.  The memory is not initialized.  If size
       is 0, then malloc() returns either NULL, or a unique pointer
       value that can later be successfully passed to free().

Learn more here : <a href="https://man7.org/linux/man-pages/man3/free.3.html">man malloc</a>

<hr>
I hope you found it interesting! <br>
And if you are going to do get_next_line, I wish you good luck and hope that you learned something here!
