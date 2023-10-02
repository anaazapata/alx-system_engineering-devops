# **Shell, I/O Redirection**

I = Input

O = Output

Standard Input, Output, and Error:

On Unix system “everything is a file”, and when we use commands (programs) such as ls, that command send their results to a special file called standard output (stdout) and their status messages to another file called standard error (stderr). By default, both standard output and standard error are linked to the screen and not saved into a disk file.

So for example if we want to save the list of file we have in a long format, we can redirect on where we want to save it, so if we want to save our list file in a file named “my_list” we can always redirect this output to the file “my_list.”

It is useful to store output of a command in a file, we won’t see the output on the screen but we can see it on the file we just createad and redirected our stdout.

So, here the input is `ls -l` itself and the output is our long format list.

- What do the commands `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr` do

| Command | What is doing? |
| --- | --- |
| head | Prints the first 10 lines of a file |
| tail | Output the last part of a file |
| find | It searches for files and directories in a directory hierarchy. |
| wc | word count, is used to display the number of lines, words, and bytes contained in files. |
| sort | Sort lines of text |
| uniq | Report or omit repeated lines |
| grep | Print lines matching a pattern |
| tr | translates or delete characters from stdin and writes the result yo stdout |
- How to redirect standard output to a file

The way we can redirect stdout to a file is by connecting command together into command pipelines and example of this is when we may want to display the text of a file but not in our screens so we can redirect the command less to a file like this:

`**less ls-output.txt**`

- How to get standard input from a file instead of the keyboard

Using the < redirection operator, we can Chang the source of stdin from the keyboard.

- How to send the output from one program to the input of another program

With pipelines denoted by this command | 

Filtres take input, change it and then output it. We can combine several commands together like this:

**`ls /bin /usr/bin | sort | less`**
