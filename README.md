Tis is the README file for ALX project: C - SIMPLE SHELL
C | GROUP PROJECT | SYSCALL

BACKGROUND CONTEXT
Write a simple UNIX command interpreter.

LEARNING OBJECTIVES
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

GENERAL
Who designed and implemented the original Unix operating system
Who wrote the first version of the UNIX shell
Who invented the B programming language (the direct predecessor to the C programming language)
Who is Ken Thompson
How does a shell work
What is a pid and a ppid
How to manipulate the environment of the current process
What is the difference between a function and a system call
How to create processes
What are the three prototypes of main
How does the shell use the PATH to find the programs
How to execute another program with the execve system call
How to suspend the execution of a process until one of its children terminates
What is EOF / “end-of-file”?

REQUIREMENTS
GENERAL
1. Allowed editors: vi, vim, emacs
2. All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options *-Wall -Werror -Wextra -pedantic -std=gnu89*
2. All your files should end with a new line
3. A README.md file, at the root of the folder of the project is mandatory
4. Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
5. Your shell should not have any memory leaks
6. No more than 5 functions per file
6. All your header files should be include guarded
7. Use system calls only when you need to (why?)
8. Write a README with the description of your project
9. You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker

GITHUB
*There should be one project repository per group. If you and your partner have a repository with the same name in both your accounts, you risk a 0% score. Add your partner as a collaborator.*

COMPILATION
Your shell will be compiled this way:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh


0. Betty would be proud
mandatory
Write a beautiful code that passes the Betty checks

1. Simple shell 0.1
mandatory
Write a UNIX command line interpreter.

2. Simple shell 0.2
mandatory
Simple shell 0.1 +

Handle command lines with arguments

3. Simple shell 0.3
mandatory
Simple shell 0.2 +

Handle the PATH
fork must not be called if the command doesn’t exist

4. Simple shell 0.4
mandatory
Simple shell 0.3 +

Implement the exit built-in, that exits the shell
Usage: exit
You don’t have to handle any argument to the built-in exit

5. Simple shell 1.0
mandatory
Simple shell 0.4 +

Implement the env built-in, that prints the current environment

6. Simple shell 0.1.1
#advanced
Simple shell 0.1 +

Write your own getline function
Use a buffer to read many chars at once and call the least possible the read system call
You will need to use static variables
You are not allowed to use getline

7. Simple shell 0.2.1
#advanced
Simple shell 0.2 +

You are not allowed to use strtok

8. Simple shell 0.4.1
#advanced
Simple shell 0.4 +

handle arguments for the built-in exit
Usage: exit status, where status is an integer used to exit the shell

9. setenv, unsetenv
#advanced
Simple shell 1.0 +

Implement the setenv and unsetenv builtin commands

10. cd
#advanced
Simple shell 1.0 +

Implement the builtin command cd:

11. ;
#advanced
Simple shell 1.0 +

Handle the commands separator ;

12. && and ||
#advanced
Simple shell 1.0 +

Handle the && and || shell logical operators

13. alias
#advanced
Simple shell 1.0 +

Implement the alias builtin command
Usage: alias [name[='value'] ...]
alias: Prints a list of all aliases, one per line, in the form name='value'
alias name [name2 ...]: Prints the aliases name, name2, etc 1 per line, in the form name='value'
alias name='value' [...]: Defines an alias for each name whose value is given. If name is already an alias, replaces its value with value

14. Variables
#advanced
Simple shell 1.0 +

Handle variables replacement
Handle the $? variable
Handle the $$ variable

15. Comments
#advanced
Simple shell 1.0 +

Handle comments (#)

16. File as input
#advanced
Simple shell 1.0 +

Usage: simple_shell [filename]
Your shell can take a file as a command line argument
The file contains all the commands that your shell should run before exiting
The file should contain one command per line
In this mode, the shell should not print a prompt and should not read from stdin
