# Shell Scripts Description. 
> What each script is doing?

**0-current_working_directory**
: command pwd, that prints the absolute path name of the CWD.

**1-listit**
: command ls, that displays the contents list of your current directory.

**2-bring_me_home**
: command cd: changes the working directory to the user's home directory.

**3-listfiles**
: command ls -lm displays current directory contents in a long format.


**4-listmorefiles**
: command ls -la Display current directory contents, including hidden files (starting with .). 

**5-listfilesdigitonly**
: command ls -all Display current directory contents:
* Long format
* with user and group IDs displayed numerically
* hidden files (starting with .)


**6-firstdirectory**
: command mkdir creates a directory named my_first_directory in the /tmp/ directory.


**7-movethatfile**
: command mv move the file betty from /tmp/ to /tmp/my_first_directory.


**8-firstdelete**
: command rm delete the file betty which is in /tmp/my_first_directory.


**9-firstdeletion**
: command rm -r delete the directory my_first_directory that is in the /tmp directory.


**10-back**
: command cd - that changes the working directory to the previous one


**11-lists**
: command ls -la . .. /boot lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.


**12-file_type**
: command file prints the type of the file named iamafile.

**13-symbolic_link**
: commmand ln -s /bin/ls __ls__  symbolic link to /bin/ls, named __ls__. 


**14-copy_html**
: command cp *u.html .. copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.


**100-lets_move**
: command mv [[:uppercase:]]* /tmp/u


**101-clean_emacs**
: command rm *~ deletes all files in the current working directory that end with the character ~ .


**102-tree**
: command mkdir -p creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.


**103-commas**
: command ls -pmav  lists all the files and directories of the current directory, separated by commas (,).


**school.mgc**
: magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0.
