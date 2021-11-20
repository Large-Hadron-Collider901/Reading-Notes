# FileIO & Exceptions 

## Reading and Writing Files in Python

#### What Is a File?

A file is a group of bytes that are used to store data. This data is organized according to it's specific format. Types of format can be as basic as a text file or as complex as a program executable. The bytes are translated into binary so they can be processed by the computer.

Files consist of three main parts:

1. *Header*: Includes metadata about the contents of the file (file name, size, format, etc.)

2. *Data*: Contents of the file written by the creator or editor.

3. *End of file (EOF)*: Special characters that represent the end of a file.

#### File Paths

A file path is a string that represents the file's location snd consists of three main parts:

1. Folder Path: the file folder location on the file system where folders are separated by a forward slash / (Unix) or a backslash \ (Windows).

2. File Name: The name of the file.

3. Extension: the end of the file path is represented by a period (.) followed by the file type (for example: a text file ends in .txt)


#### Opening and Closing Files in Python


There are multiple ways to open and close a file in python, the most common ways include: 

1. try-finally method
2. with statement method

```
# Try-Finally method: 

reader = open('your_file.txt')
try:
    # further file processing code will go here
finally:
    reader.close()
   
# OR

# With statement method

with open('your_file.txt') as reader:
    # further file processing code will go here`

# The with statement automatically takes care of closing the file

```

Additionally, you will likely want to use a second positional argument called `mode`. The `mode` argument consists of a string that represents how you are using the file that you want to opne. The default is 'r', which opens the file in read-only mode as a text file. The `mode` argument should be placed inside your parenthesis next to your file and seperated with a comma like so:

`open('your_file.txt', 'r')`

Commonly used options for `mode` include:

* `r` = Open for reading(default)
* `w` = Open for writing, truncating(overwriting) the file first
* `rb` = Open in binary mode (read using byte data)
* `wb` = Open in binary mode (write using byte data)

#### Reading and Writing Opened Files

There are several methods that can be used to read or write to the file, here are some common methods:

* `.read(size=-1)` This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the whole file is read.

* `.readline(size=-1)` This reads at most size number of characters from the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.

## Introduction To Python Exceptions

An **exception error* is a type of error that occurs whenever syntactically correct Python code results in an error. When an exception error occurs, rather than showing the message `exception error`, Python details the type of exception that was encountered



**Reading Sources:** [Reading-and-Writing-Files-in-Python-(Guide)](https://realpython.com/read-write-files-python/)
[Python-Exceptions:-An-Introduction](https://realpython.com/python-exceptions/)