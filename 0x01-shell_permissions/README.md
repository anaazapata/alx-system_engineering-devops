Linux is a multitasking operating system but also are multi-user OS. One that more users can have access to the same computer simultaneously.

- `u` - The file owner.
- `g` - The users who are members of the group.
- `o` - All other users.
- `a` - All users, identical to `ugo`.

- What do the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do

chmod → modify access rights

sudo → temporarily become the superuser

su →temporarily become the superuser

chown → change file ownership

chgrp → changes a file group ownership

- Linux file permissions

Files and directories have access rights for the file owner, group files, and everybody else.

You can assign a right just for reading, writing, executing a file, or all of the 3 assignations. 

If we use the ls -l ← long format list command, we can see the rights a file or directory have

![Captura de Pantalla 2022-10-06 a la(s) 10.08.21.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f2b2dd99-d619-43af-8d8e-4870e70447c0/Captura_de_Pantalla_2022-10-06_a_la(s)_10.08.21.png)

- How to represent each of the three sets of permissions (owner, group, and other) as a single digit
- `r` (read) = 4
- `w` (write) = 2
- `x` (execute) = 1
- no permissions = 0

- How to change permissions, owner and group of a file

With the chmod command we can change the permissions of a file or directory.

![Captura de Pantalla 2022-10-06 a la(s) 10.16.34.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cde6f54f-bc81-451e-b144-ffa06c618340/Captura_de_Pantalla_2022-10-06_a_la(s)_10.16.34.png)

![Captura de Pantalla 2022-10-06 a la(s) 10.16.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/216bf98b-f3f2-48a6-ae65-f13c7336e155/Captura_de_Pantalla_2022-10-06_a_la(s)_10.16.47.png)

- Why can’t a normal user `chown` a file

`chown` is a privilege restricted to root since, otherwise, you could pawn off your files on other users to avoid quota restrictions.

- How to run a command with root privileges

su and sudo can give us root privileges.

`su` → by typing this command, we will be prompted with the superuser’s password to exit; just type **exit.**

`sudo` → one or more users can have superuser’s privileges format: `sudo command`

- How to change user ID or become superuser

# **Other Man Pages**

- How to create a user

`useradd [OPTIONS] USERNAME`

Linux:

`sudo useradd username`

To log in as the newly created user, you need to set the user password. To do that, run the `[passwd](https://linuxize.com/post/how-to-change-user-password-in-linux/)` command followed by the username:

```
sudo passwd username
```

- How to create a group

1. To create a new group, use the **groupadd** command.Type the following command:

`groupadd -g *group-ID* *group-name*`where *group-ID* is the numeric identifier of the group, and *group-name* is the name of the group. 
2. To add a member to a supplementary group, use the **usermod** command to list the supplementary groups that the user is currently a member of, and the supplementary groups that the user is to become a member of.For example, if the user is already a member of the group `groupa`, and is to become a member of `groupb`, use the following command:

`usermod -G groupa,groupb *user-name*`where *user-name* is the user name. 
3. To display who is a member of a group, use the **getent** command.Type the following command:

`getent group *group-name*`where *group-name* is the name of the group. 
4. To remove a member from a supplementary group, use the **usermod** command to list the supplementary groups that you want the user to remain a member of.For example, if the user's primary group is `users` and the user is also a member of the groups `mqm`, `groupa` and `groupb`, to remove the user from the `mqm` group, use the following command:

`usermod -G groupa,groupb *user-name*`where *user-name* is the user name.

-IBM (s.f)

[Creating and managing groups on Linux](https://www.ibm.com/docs/en/ibm-mq/9.1?topic=windows-creating-managing-groups-linux)

- How to print real and effective user and group IDs

`id - print real and effective user and group IDs`

- How to print the groups a user is in

 `groups - print the groups a user is in`

- How to print the effective userid

`whoami : Print effective user id`

Resources.

[](https://linuxize.com/post/how-to-create-users-in-linux-using-the-useradd-command/)

[](https://linuxize.com/post/understanding-linux-file-permissions/)
