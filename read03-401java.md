# Java Primitives versus Objects

- Pros and Cons : the amount of available memory and what default values we should handle.
- Single Item Memory Footprint : 
`boolean – 1 bit`
`byte – 8 bits`
`short, char – 16 bits`
`int, float – 32 bits`
`long, double – 64 bits`

These values can vary according to Virtual Machine implementation.


# Exceptions

occurs during the execution of a program called an exception object contains information about error and the stats of the program.and  exception handler chosen is said to catch the exception.

### there are three kinds of Exceptions:

- java.io.FileReader : if the user enter incorrect name file will appear java.io.FileNotFoundException.
- java.io.IOError : unable to read the file because of a hardware or system malfunction.
- FileReader : If a logic error causes a null to be passed to the constructor, the constructor will throw NullPointerException.

### Scanner

Scanner also supports tokens for all of the Java language's primitive kinds except `char`.

Scanner is a utility class in java.util package which can parse primitive types and strings using regular expressions. It can read text from any object which implements the Readable interface.



