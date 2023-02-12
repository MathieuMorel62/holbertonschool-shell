# <p align="center">SHELL, PERMISSIONS</p>

<img src="https://cdn.mindmajix.com/blog/images/linux-file-permissions-07092020.png" width="100%">

## Description
### Shell Permissions

Shell permissions determine who can do what with a file or directory on the operating system. Permissions can be set for three different groups of users: the file owner, the group associated with the file, and everyone.

### Types of Permissions

There are three types of Shell permissions: read, write, and execute.

- Read permission (`r`) allows a user to read the contents of a file or list the files in a directory.
- Write permission (`w`) allows a user to modify the contents of a file or create new files in a directory.
- Execute permission (`x`) allows a user to run a file as a program.

### Permission Commands

Here are the basic commands for managing permissions in Shell:
  
- `chmod`: Changes the permissions of a file or directory
- `chown`: Changes the owner of a file or directory
- `chgrp`: Changes the group associated with a file or directory
  
It's important to understand Shell permissions to ensure that important files and directories are protected and that users can access the files and directories they need to do their work.

### Conclusion
  
In conclusion, Shell permissions allow for controlling who can do what with the files and directories on the operating system. The types of permissions include read, write, and execute, and the permission commands allow for managing these permissions for different users. Understanding Shell permissions is important for ensuring the security and functionality of the operating system.

## Resources
### Read or Watch:

- [Permissions](https://intranet.hbtn.io/rltoken/UL7cEzRpzknNKTQ-3-zH2w)

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All your scripts will be tested on Ubuntu 20.04 LTS
- All your scripts should be exactly two lines long (`$ wc -l file` should print 2)
- All your files should end with a new line ([why?](http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789))
- The first line of all your files should be exactly `#!/bin/bash`
- A `README.md` file, at the root of the folder of the project, describing what each script is doing
- You are not allowed to use backticks, `&&`, `||` or `;`
- All your files must be executable

-----------------------

# TASKS

### [0. My Name Is Betty](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/0-iam_betty)

Create a script that switches the current user to the user `betty`.
- You should use exactly 8 characters for your command (+1 character for the new line)
- You can assume that the user `betty` will exist when we will run your script
```c
mathieu@ubuntu:/tmp/h$ tail -1 0-iam_betty | wc -c
9
mathieu@ubuntu:/tmp/h$
```

----------------------

### [1. Who Am I](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/1-who_am_i)

Write a script that prints the effective username of the current user.
```c
mathieu@ubuntu:/tmp/h$ ./1-who_am_i
mathieu
mathieu@ubuntu:/tmp/h$ 
```

-----------------------

### [2. Groups](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/2-groups)

Write a script that prints all the groups the current user is part of.
```
mathieu@ubuntu:/tmp/h$ ./2-groups
mathieu adm cdrom sudo dip plugdev lpadmin sambashare
mathieu@ubuntu:/tmp/h$ 
```
Note: depending on the user, you will get a different output.

-----------------------

### [3. New Owner](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/3-new_owner)

Write a script that changes the owner of the file `hello` to the user `betty`.
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 mathieu mathieu 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 mathieu mathieu  0 Sep 20 14:18 hello
mathieu@ubuntu:/tmp/h$ sudo ./3-new_owner 
mathieu@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 mathieu mathieu 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 betty  mathieu  0 Sep 20 14:18 hello
mathieu@ubuntu:/tmp/h$
```

----------------------

### [4. Empty !](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/4-empty)

Write a script that creates an empty file called `hello`.

----------------------

### [5. Execute](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/5-execute)

Write a script that adds execute permission to the owner of the file `hello`.
- The file `hello` will be in the working directory
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:26 5-execute
-rw-rw-r-- 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./hello
bash: ./hello: Permission denied
mathieu@ubuntu:/tmp/h$ ./5-execute 
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:26 5-execute
-rwxrw-r-- 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

-----------------------

### [6. Multiple Permissions](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/6-multiple_permissions)

Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello`.
- The file `hello` will be in the working directory
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 36 Sep 20 14:31 6-multiple_permissions
-rw-r----- 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./6-multiple_permissions 
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 36 Sep 20 14:31 6-multiple_permissions
-rwxr-xr-- 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

------------------------------

### [7. Everybody !](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/7-everybody)

Write a script that adds execution permission to the owner, the group owner and the other users, to the file `hello`
- The file `hello` will be in the working directory
- You are not allowed to use commas for this script
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:35 7-everybody
-rw-r----- 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./7-everybody 
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:35 7-everybody
-rwxr-x--x 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

-------------------------

### [8. James Bond](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/8-James_Bond)

Write a script that sets the permission to the file `hello` as follows:
- Owner: no permission at all
- Group: no permission at all
- Other users: all the permissions

The file `hello` will be in the working directory You are not allowed to use commas for this script
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:40 8-James_Bond
-rwxr-x--x 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./8-James_Bond 
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 28 Sep 20 14:40 8-James_Bond
-------rwx 1 mathieu mathieu 23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

------------------------

### [9. John Doe](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/9-John_Doe)

Write a script that sets the mode of the file `hello` to this :
```c
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
``` 

- The file `hello` will be in the working directory 
- You are not allowed to use commas for this script

------------------------

### [10. Look In The Mirror](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/10-mirror_permissions)

Write a script that sets the mode of the file `hello` the same as `olleh`’s mode.
- The file `hello` will be in the working directory
- The file `olleh` will be in the working directory
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 42 Sep 20 14:45 10-mirror_permissions
-rwxr-x-wx 1 mathieu mathieu 23 Sep 20 14:25 hello
-rw-rw-r-- 1 mathieu mathieu  0 Sep 20 14:43 olleh
mathieu@ubuntu:/tmp/h$ ./10-mirror_permissions 
mathieu@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 mathieu mathieu 42 Sep 20 14:45 10-mirror_permissions
-rw-rw-r-- 1 mathieu mathieu 23 Sep 20 14:25 hello
-rw-rw-r-- 1 mathieu mathieu  0 Sep 20 14:43 olleh
mathieu@ubuntu:/tmp/h$ 
```

Note: the mode of `olleh` will not always be 664. Make sure your script works for any mode.

---------------------------

### [11. Directories](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/11-directories_permissions)

Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 20
-rwxrwxr-x 1 mathieu mathieu   24 Sep 20 14:53 11-directories_permissions
drwx------ 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx------ 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx------ 2 mathieu mathieu 4096 Sep 20 14:49 dir2
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./11-directories_permissions 
mathieu@ubuntu:/tmp/h$ ls -l
total 20
-rwxrwxr-x 1 mathieu mathieu   24 Sep 20 14:53 11-directories_permissions
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir2
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$
```

----------------------------

### [12. More Directories](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/12-directory_permissions)

Create a script that creates a directory called `my_dir` with permissions 751 in the working directory.
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 20
-rwxrwxr-x 1 mathieu mathieu   39 Sep 20 14:59 12-directory_permissions
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir2
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ ./12-directory_permission s
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu   39 Sep 20 14:59 12-directory_permissions
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir2
drwxr-x--x 2 mathieu mathieu 4096 Sep 20 14:59 my_dir
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

----------------------------

### [13. Change Group](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/13-change_group)

Write a script that changes the group owner to `school` for the file `hello`
- The file hello will be in the working directory
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu   34 Sep 20 15:03 13-change_group
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir2
drwxr-x--x 2 mathieu mathieu 4096 Sep 20 14:59 my_dir
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ sudo ./13-change_group 
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu      34 Sep 20 15:03 13-change_group
drwx--x--x 2 mathieu mathieu    4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu    4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu    4096 Sep 20 14:49 dir2
drwxr-x--x 2 mathieu mathieu    4096 Sep 20 14:59 my_dir
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

---------------------------

### [14. Owner And Group](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/14-change_owner_and_group)

Write a script that changes the owner to `vincent` and the group owner to `staff` for all the files and directories in the working directory.
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu   36 Sep 20 15:06 14-change_owner_and_group
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir0
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir1
drwx--x--x 2 mathieu mathieu 4096 Sep 20 14:49 dir2
drwxr-x--x 2 mathieu mathieu 4096 Sep 20 14:59 my_dir
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ sudo ./14-change_owner_and_group 
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 vincent staff   36 Sep 20 15:06 14-change_owner_and_group
drwx--x--x 2 vincent staff 4096 Sep 20 14:49 dir0
drwx--x--x 2 vincent staff 4096 Sep 20 14:49 dir1
drwx--x--x 2 vincent staff 4096 Sep 20 14:49 dir2
drwxr-x--x 2 vincent staff 4096 Sep 20 14:59 my_dir
-rw-rw-r-- 1 vincent staff   23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

----------------------------

### [15. Symbolic Links](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/15-symbolic_link_permissions)

Write a script that changes the owner and the group owner of `_hello` to `vincent` and `staff` respectively.
- The file `_hello` is in the working directory
- The file `_hello` is a symbolic link
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu   44 Sep 20 15:12 15-symbolic_link_permissions
-rw-rw-r-- 1 mathieu mathieu   23 Sep 20 14:25 hello
lrwxrwxrwx 1 mathieu mathieu    5 Sep 20 15:10 _hello -> hello
mathieu@ubuntu:/tmp/h$ sudo ./15-symbolic_link_permissions 
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu      44 Sep 20 15:12 15-symbolic_link_permissions
-rw-rw-r-- 1 mathieu mathieu      23 Sep 20 14:25 hello
lrwxrwxrwx 1 vincent  staff    5 Sep 20 15:10 _hello -> hello
mathieu@ubuntu:/tmp/h$ 
```

---------------------------

### [16. If Only](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/16-if_only)

Write a script that changes the owner of the file `hello` to `vincent` only if it is owned by the user `guillaume`.
- The file `hello` will be in the working directory
```c
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu    mathieu      47 Sep 20 15:18 16-if_only 
-rw-rw-r-- 1 guillaume mathieu      23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ sudo ./16-if_only 
mathieu@ubuntu:/tmp/h$ ls -l
total 24
-rwxrwxr-x 1 mathieu mathieu      47 Sep 20 15:18 16-if_only 
-rw-rw-r-- 1 vincent  mathieu      23 Sep 20 14:25 hello
mathieu@ubuntu:/tmp/h$ 
```

---------------------------------------

## Author

- Mathieu Morel
