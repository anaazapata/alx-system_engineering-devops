# Projects:
[Shell, Basics](#0x00-shell_basics)

[Shell, permissions](#0x01-shell_permissions)

[Shell, I/0 Redirections and filters](#0x02-shell_redirections)



## [Shell, Basics](#0x00-shell_basics)

> Shell, basics project is about knowning the Shell (bash) and how it takes commands from the keyboard and gives them to the operating system, at the same time we get to know the Terminal who acts as an emulator between us and the shell, the Terminal let us interact with the shell.

This directory contains shell scripts, since shell scripts is an important part of process automation in Linux. Scripting help us wirte a sequence of commands in a file and then execute them.

Commands used in the shell scripts:
* `pwd`
* `cd`
* `ls`
* `less`
* `file`
* `ln`
* `cp`
* `mv`
* `rm`
* `mkdir`
* `type`
* `which`
* `help`
* `man`

Inside the directory 0x00-shell_basics we can find the description of what each script is doing.


## [Shell, permissions](#0x01-shell_permissions)
> Linux is a multitasking operating system but also is a multi-user OS. More than one user can have access to the same computer simultaneously through permissions.

This directory contains shell permission scripts.

Commands used in the shell scripts:

* `chmod`
* `sudo`
* `su`
* `chown`
* `chgrp`
* `id`
* `groups`
* `whoami`
* `adduser`
* `useradd`
* `addgroup`


## [Shell, I/0 Redirections and filters](#0x02-shell_redirections)
> On Unix system “everything is a file”, and when we use commands (programs) such as ls, that command send their results to a special file called standard output (stdout) and their status messages to another file called standard error (stderr). By default, both standard output and standard error are linked to the screen and not saved into a disk file.

This directory contains shell redirection scripts

Commands used in the shell scripts:

* `echo`
* `cat`
*`head`
* `tail`
* `find`
* `wc`
* `sort`
* `uniq`
* `grep`
* `tr`
* `rev`
* `cut`
* `passwd` (5) (i.e. man 5 `passwd`)


## [Shell, init files, variables and expansions](#0x03-shell_variables_expansions)
> A Shell Initialization file is a Shell script that runs automatically each time the Shell executes. We have 3 types of Shell and Shell Initialization Files are used respectevely: interactive non-login Shell, interactive login Shell and non interactive Shell.

This directory contains shell init files, variables and expansions

* `printenv`
* `set`
* `unset`
* `export`
* `alias`
* `unalias`
* `.`
* `source`
* `printf`

