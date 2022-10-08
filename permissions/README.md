# SHELL, PERMISSIONS

![img](https://cdn.mindmajix.com/blog/images/linux-file-permissions-07092020.png)


## RESOURCES

### Read or watch:

- [Permissions](https://intranet.hbtn.io/rltoken/UL7cEzRpzknNKTQ-3-zH2w)

-----------------------

# TASKS


[0. MY NAME IS BETTY](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/0-iam_betty)

Create a script that switches the current user to the user betty.

  - You should use exactly 8 characters for your command (+1 character for the new line)

  - You can assume that the user betty will exist when we will run your script

----------------------

[1. WHO AM I](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/1-who_am_i)

Write a script that prints the effective username of the current user.

-----------------------

[2. GROUPS](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/2-groups)

Write a script that prints all the groups the current user is part of.

-----------------------

[3. NEW OWNER](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/3-new_owner)

Write a script that changes the owner of the file hello to the user betty.

----------------------

[4. EMPTY !](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/4-empty)

Write a script that creates an empty file called hello.

----------------------

[5. EXECUTE](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/5-execute)

Write a script that adds execute permission to the owner of the file hello.

  - The file hello will be in the working directory

-----------------------

[6. MULTIPLE PERMISSIONS](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/6-multiple_permissions)

Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

  - The file hello will be in the working directory

------------------------------

[7. EVERYBODY !](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/7-everybody)

Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello

  - The file hello will be in the working directory

  - You are not allowed to use commas for this script

-------------------------

[8. JAMES BOND](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/8-James_Bond)

Write a script that sets the permission to the file hello as follows:

  - Owner: no permission at all
      
  - Group: no permission at all

  - Other users: all the permissions

The file hello will be in the working directory You are not allowed to use commas for this script

------------------------

[9. JOHN DOE](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/9-John_Doe)

Write a script that sets the mode of the file hello to this :

    -rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello

  - The file hello will be in the working directory 

  - You are not allowed to use commas for this script

------------------------

[10. LOOK IN THE MIRROR](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/10-mirror_permissions)

Write a script that sets the mode of the file hello the same as olleh’s mode.

  - The file hello will be in the working directory

  - The file olleh will be in the working directory

Note: the mode of olleh will not always be 664. Make sure your script works for any mode.

---------------------------

[11. DIRECTORIES](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/11-directories_permissions)

Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.

----------------------------

[12. MORE DIRECTORIES](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/12-directory_permissions)

Create a script that creates a directory called my_dir with permissions 751 in the working directory.

----------------------------

[13. CHANGE GROUP](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/13-change_group)

Write a script that changes the group owner to school for the file hello

  - The file hello will be in the working directory

---------------------------

[14. OWNER AND GROUP](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/14-change_owner_and_group)

Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

----------------------------

[15. SYMBOLIC LINKS](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/15-symbolic_link_permissions)

Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.

  - The file _hello is in the working directory

  - The file _hello is a symbolic link

---------------------------

[16. IF ONLY](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/permissions/16-if_only)

Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.

  - The file hello will be in the working directory


