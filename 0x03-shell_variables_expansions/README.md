# SHELL, INIT FILES, VARIABLES AND EXPANSIONS.
> A Shell Initialization file is a Shell script that runs automatically each time the Shell executes.
We have 3 types of Shell and Shell Initialization Files are used respectevely, for example:

- Interactive non-login Shell: this Shell allow us to interact with the initialization files and execute commands introduced by the keyboard.
- Interactive login Shell: when the user login into the system, after introducing username and password, the Shell will appear and it will interact we us.
- Non Interactive Shell: this Shell only executes commands from a file or script.

### Variables

Variable: name given to a memory Location that is used to stores values in a program, it stores information that can be called and manipúlate wherever needed in the program.

Scope: the part of the program where the variable is accessible, based on the scope, it is two types: local and global.

Variable names can contain only letters (a to z or A to Z), numbers (0 to 9) or the underscore character (_)

Unix Shell variables will have their names in UPPERCASE

No spaces before or after the = sign.

Global variable: available in all shells, in can be accesed in the entire program.

Local variable: available when the scope of the variable is within the function where it is declared.

- What is a reserved variable

Variable names that we can use, because they’re reserved by Bash.

- How to create and detele variables
```bash
VARNAME="value"
```
Examples:
```bash
user1-> MYVAR1="2"
user1-> echo $MYVAR1
2
```

- What are the roles of the following reserved variables: HOME, PATH, PS1
```bash
HOME="The current user's home directory; the default for cd buil-in"
PATH="A colon-separated list of directories in which the shell looks for commands"
PS1="The primary promp string. the default value is "'\s-\v\$'""
```

### Expansion

- What is expansion and how to use them

When a command is given the first thing is that the interpreter is going to split into tokens.

When we use variables in Shell Scripts for example:

```bash
NAME="Ana"
echo hello "${NAME} !!!"
```

Each of the above tokens (echo, hello, name) NAME is expanded and replaced with “Ana”, then quotes are removed.

And finally the command is then interpreted.


### Alias

Alias command allow us to create simple names for commands, so we can create an easy name to perform commands that are complex and we can use them in the same way that ordinary commands are used.

- How to create an alias

`alias [-p] [name=”value”]`

- How to list aliases

When we use `alias` without -p option, alias provides a list of aliases that are in effect for the current user.

How to temporarily disable an alias
`/aliasname`
