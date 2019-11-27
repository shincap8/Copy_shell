<h1 align ="center"> _SHELL() </h1><br>

## Table of Contents 
---
- [Authors](#authors)
- [Introduction](#introduction)
- [Description](#description)
- [Installation](#installation)
- [Test](#Test)
- [Files](#files)
- [Features](#features)
- [Built With](#built-with)
- [Acknowledgments](#acknowledgments)
---
## Authors 
---
* [Kevin Giraldo](https://twitter.com/KevinGiraldo89)
* [Sara Hincapié](https://twitter.com/SaraHincapiMon1)
---
## Introduction
> Project for the end of the first trimester at Holberton School. This project is for us to show what we have learnt in C during these 3 months, the use of loops, conditional, macros, structures, variables, pointers and more, also to test our teamwork skills and our work under pressure.
---
## Description 
---
The _shell() compatible command language interpreter that executes commands read from the standard input or from a file.
---
## Installation 
---
In order to run the shell command interpreter, you must install it in your repository by cloning the following (shown below) in your machine running:
```
git clone direccion del repositorio final
```
---
## Test
---
- In order to compile the function you must run the following line in your shell:
```
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```
_Note_: there are two ways of using the command interpreter:

#### Interactive mode:
```
 $ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
#### Non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```
---
- To read the manual you man run:
```man ./[FILE]``` taking into account the structure, for our case it would be ```man ./man_hsh```

| File Name | Description and contents |
| --- | --- |
| [manpage](man_1_simple_shell) | This is the manpage for the shell command, this will help us know how to use the shell and the many uses of it, in here we can find examples and the correct sintaxis of the commands.|
| [_library.h](library.h) |This is the headers file where we can find all the prototypes of our functions and the structures used. |
| [_stdlib.c](_stdlib.c) |In here we have the atoi function it is used to make integers into characters. |
| [_string.c](_string.c) |Here we can find the function _strtok that splits a string with a delimiter given and the _strcat function that concatenates two strings given. |
| [main.c](main.c) |This function has the launch function who starts all the process. |
| [shell.c](shell.c) |In this file there are 5 functions the launch function who manage the other functions, clearNprint function prints the prompt of the shell, parse function saves each string worth of saving after it is divided with the strtok function, findpath function searches for the path in the environment list where the command typed can be executed|
---
## Features 

A simple shell must work with the path and without the path
* /bin/ls
* ls
---
### Examples of use

Below you can find use of some commands.

```
$ ls -a
$ echo Hola
$ pwd
```
Here are the result of this actions:

```
Image of the console using the commands above
```


## Built With

* [C](https://en.wikipedia.org/wiki/C_(programming_language))
* [Vim](https://https://en.wikipedia.org/wiki/Vim_(text_editor)/)
* [Vagrant](https://www.vagrantup.com/)
* [Peppermint](https://www.osboxes.org/peppermint/) Need to change to what Kevin is using
* [Ubuntu](https://www.ubuntu.com/)
* [GCC 4.8.4 Compiler](https://gcc.gnu.org/)
