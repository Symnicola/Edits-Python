The Python Traceback in General

There are several sections to every Python traceback that are important. The diagram below was an attempt to help you see those different parts.

![python_traceback_diagram.webp](attachment:python_traceback_diagram.webp)

In python, it is best to read the traceback from the bottom moving up. The last line of the traceback I call the error message line, and it contains the exceptions name which was raised (outlined in blue). After, the exception name is the error message (outlined in yellow). This message usually contains helpful information for understanding the reason for the exception being raised. Moving up the traceback (out-lined in green) is the different function calls moving from bottom to top, most recent to least recent. Two-line entries represent these calls for each call. The first line of each call contains information like the file name, line number, and module name, all specifying where the code can be found. The second line for these calls includes the actual code that was executed (underline in red). There are differences between tracebacks output when executing your code in the command-line and running code in the REPL. Below is the same code from the previous section executed in a `REPL` and the resulting traceback output.


Python


```python
>>> def greet( someone ):
>>>
...   print('Hello, ' +someon)
... 
>>> greet("Chad")

Traceback (most recent call last):
  File "", line 1, in 
  File "", line 2, in greet
NameError: name 'someon' is not defined
```
```


      File "<ipython-input-2-63d2be34fe0d>", line 7
        Traceback (most recent call last):
                        ^
    SyntaxError: invalid syntax




```python

```
