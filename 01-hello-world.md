# Hello World

## Introduction to C++
- created by [Bjarne stroustrup](https://en.wikipedia.org/wiki/Bjarne_Stroustrup) at bell labs in 1979
- derived from C with a goal of adding OOP

#### Why learn
- fast
- flexible
- cross platform support
- it's new thinking

#### writing the first program
- files alway have a **.cpp** extension
- code is executed line by line, from top to bottom

```cpp
#include <iostream>

int main() {
    std::cout << "Hello world\n";

    return 0;
}
```
the gist of the code above

1. First line includes libraries, for this case, its the input/output libs from standard library
2. line 2 defines the start of the `main` function, this where our program starts executing,
3. line 3, _console out_, writes to the console
4. line for defines the exit value of the main function
5. line 5 marks the end of the main function

Anything in between the main function is where our program goes.

multiple statements can be written by adding multiple line.
```cpp
std::cout << "Hello world!\n";
std::cout << "Goodbye world!\n"
```

> NOTE: "\n" is an escape character to create a new line

#### even more
- c++ is case sensitive
- comments starts with double slash **//**
- white spaces are ignored

## Compilation and execution
- needed to translate c++ programs to machine code

To compile the program, this outputs a binary file, **a.out**
```sh
g++ 01-hello-world.cpp
```

To run the file
```sh
./a.out
```

## Comments
- notes in code
- two types
    1. Single line comments
        ```cpp
        int main() {
            // this is a single line comment
            std::cout << "Hello world\n"; // can also go here
            return 0;
        }
        ```
    2. multiline
        ```cpp
        int main() {
        /* starts with a slash followed by an asteric
        it can span multiple lines
        ends with an asteric then a slash */
        std::cout << "Hello world\n";
        return 0;
        }

