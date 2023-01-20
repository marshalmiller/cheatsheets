# Getting Started with C++

Why C++?

    C++ is developed by Bjarne Stroustrup at Bell Labs in 1979.
    C++ adds object-oriented programming and many other new features to C.
    C++ is fast, flexible, and well-supported across multiple platforms.
    Being one of the most popular languages today, C++ has a wide range of applications across many fields.

C++ Style Guide

Style is what we call the conventions that govern our C++ code. These rules exist to keep the code base manageable and readable.

Here are some basic tips from Google’s C++ Style Guide:

    #include statements are mostly written at the beginning of any C/C++ program.
    Names can never start with a digit or be the same as a predefined C++ keyword.
    Types, variable, operators, and literal values should be separated by one space horizontally.
    Classes, functions, and global variables should be separated by one space vertically.
    All indentations should be two spaces at a time.

#include <iostream>
#include <string>
using namespace std;

// This program print out “Hello World!”
int main() {
  string message = "Hello World!\n";
  cout << message;
  return 0;
}

C++ Compile and Execute

C++ a compiled language, which means a compiler needs to first translate your C++ source code into machine code before it can be run. There are two common ways for running C++ programs: using the command line or an IDE.

    On the command line, type g++ and the filename to compile your program, then execute it with ./ and the name of the executable.
    On an IDE, explore external resources because the process is different depends on which IDE is being used.

