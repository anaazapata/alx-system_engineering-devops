# SHELL I/O REDIRECTIONS AND FILTERS.
> Standard Input, Output, and Error. On Unix system “everything is a file”, and when we use commands (programs) such as ls, that command send their results to a special file called standard output (stdout) and their status messages to another file called standard error (stderr). By default, both standard output and standard error are linked to the screen and not saved into a disk file.

For example if we want to save the list of file we have in a long format, we can redirect on where we want to see/save it, so if we want to see/save our list file in a file named “my_list” we can always redirect this output to the file “my_list.”

It is useful to store output of a command in a file, we won’t see the output on the screen but we can see it on the file we just createad and redirected our stdout.

So, here the input is `ls -l` itself and the output is our long format list that now we can find in our life "my_list".


**0-hello_world**
: Command echo "Hello, World", prints text followed by a new line to the STDOUT.
