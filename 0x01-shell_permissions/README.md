# Shell Permissions.
> Linux is a multitasking operating system but also multi-user OS. One that more users can have access to the same computer simultaneously.

**0-iam_betty**
: Command cd, switches the current user to the user betty.


**1-who_am_i**
: Command whoami, prints the effective username of the current user.


**2-groups**
: Command group, prints all the groups the current user is part of.


**3-new_owner**
: Command chown betty hello, chanes the owner of the file hello to the user betty.


**4-empty**
: Command touch hello, script that creates and empty filled called hello.


**5-execute**
: Command chmod u+x hello, add execute permission to the owner of the file hello.


**6-multiple_permissions**
: Command chmod ug+x,o+r hello, adds execute permission to the owner and the group owner, add read permission to other users.


**7-everybody**
: Command chmod ugo+x, adds execution permission to the owner, the group and other users.


**8-James_Bond**
: Command chmod 007 helo, sets the permission to file hellow as follows:
* Owner: no permission at all
* Group: no permission at all
* Other users: all the permissions


**9-John_Doe**
: Command chmod 753 hello, sets the mode of the file hello to this -rwxr-x-wx


**10-mirror_permissions**
: Command chmod --reference=olleh hello , sets the mode of the file hello the same as olle's


**11-directories_permissions*
: Command chmod -R a+X, adds execute permission to all the subdirectories of the current directory for the owner, group owner and all other users.


**12-directory_permissions**
: Command mkdir -m 751 my_dir, creates a directory called my_dir with permissions 751.


**13-change_group**
: Command chgrp school hello, changes the group owner to school for the file hello.


**100-change_owner_and_group**
: Command chown -R vincent:staff . changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.


**101-symbolix_link_permissiosn**
: Command chown -h vincent:staff _hello changes the owner and the group owner of _hello to vincent and staff respectively.


**102-if_only**
: Command chown --from=guillaume betty  hello, changes the owner of the fille hello to betty only if it is owned by the user guillaume.


**103-Star_Wars**
: Command telnet towel.blinkenlights.nl, play the StarWars IV episode in the terminal.
