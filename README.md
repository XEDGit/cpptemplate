# cpptemplate
A bash script to create a C++ project structure, creating classes source files and headers using Orthodox Canonical Form

## Usage
  ``` shell
 $ ~ >./cpptemplate <flags> <classname 1> [<classname n...>]
  ```

## Flags
  -v OR --verbose:
  	Adds outputs on std::cout when classes get contructed, copied or destroyed
  
  -n OR --name <value>:
  	Sets `$(NAME)` variable in Makefile to `<value>`
  
  --overwrite:
  	overwrites Makefile and classes files `.cpp` and `.hpp` with new empty version
  
  -argv:
  	add `int argc, char **argv` to main.cpp
  
  -W:
  	add flags `-Wall -Werror -Wextra` to Makefile for compilation
  
  --clean:
  	removes folders `inc` `obj` `src` `Makefile`