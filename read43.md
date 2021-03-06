# What Is a File?
- a file is a contiguous set of bytes used to store data.
-  This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable
-  Files on most modern file systems are composed of three main parts:
 1. Header: metadata about the contents of the file (file name, size, type, and so on)
 2. Data: contents of the file as written by the creator or editor
 3.End of file (EOF): special character that indicates the end of the file
 
 # File Paths:
 When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file.
 
 # Exceptions versus Syntax Errors:

### The try and except Block: Handling Exceptions:
used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program

- ![handing](https://files.realpython.com/media/try_except.c94eabed2c59.png)

# Raising:
- We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
- ![Rising](https://files.realpython.com/media/assert.f6d344f0c0b4.png)

## The else Clause:
In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

- except is used to catch and handle the exception(s) that are encountered in the try clause.
- else lets you code sections that should run only when no exceptions are encountered in the try clause.
- finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.
