# Exception Handling

- Exception is an abnormal condition that arises in a code sequence at run time.
- When an exceptional condition arises, an object representing that exception is created and thrown in the method that caused the error.
- Exceptions can be generated by :

    - Java run-time system  
         Exceptions thrown by Java relate to fundamental errors that violate the rules of Java language or the constraints of Java execution environment.
    - Can be manually generated by your code.

    Java exception handling is managed via five keywords:  
    1. ```try```
    2. ```throw```
    3. ```catch```
    4. ```throws```
    5. ```finally```

    ![Exception Figure](https://howtodoinjava.files.wordpress.com/2013/04/exceptionhierarchy3.png)  
    ![Exception Figure One](https://i.stack.imgur.com/v2NAj.png)

> Exception is recoverable.  
> Error is non-recoverable. Eg: lack of resources ➡ Our of memory.  

Under Runtime Exception
1. Arithmetic Exception
2. Null Pointer Exception

## Uncaught Exceptions:

    class Exception{
        public static void main(String[] args){
            int d = 0;
            int a = 42 / d; 
        }
    }


## Array Out of Bound Exception

Here, java runtime system detects the attemps to divide by zero, it constructs a new exception object and then throws this exception. This causes the execution of Exception class to stop because once an exception has been thrown , it must be caught by an exception handler and dealed with immediately.  
Here we haven't supplied any exception handlers of our own, so the exception is caught by the default handler provided by Java Runtime System.


