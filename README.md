<img src="https://korben.info/app/uploads/2020/02/more-like-linux-wallpaper.png" width="100%">

## Description
### The Shell

The shell is a powerful tool that allows you to interact with your computer's operating system.

### What is a Shell?

A shell is a command-line interface that provides access to the underlying operating system. With the shell, you can perform tasks such as navigating the file system, managing files and directories, and running programs.

### Key Features of the Shell

- **Command Line Interface:** The shell provides a text-based interface for interacting with the operating system, making it a powerful tool for automation and scripting.
- **File System Navigation:** The shell allows you to navigate the file system and manage files and directories using commands such as `ls` and `cd`.
- **Scripting:** You can use the shell to write scripts to automate repetitive tasks, making it a powerful tool for system administration and data processing.
- **Customization:** The shell can be customized to suit your needs, with features such as aliases, environment variables, and custom prompt.

### How to Use the Shell

1. Open the shell on your computer
2. Type commands to interact with the operating system
3. Navigate the file system and manage files and directories
4. Write scripts to automate tasks
5. Customize the shell to suit your needs

### Best Practices for Using the Shell

- Learn basic commands for navigating the file system and managing files and directories
- Write clear and concise scripts for automating tasks
- Use aliases and environment variables to make the shell easier to use
- Invest in learning the shell and familiarize yourself with its features
   
By using the shell, you can become more efficient and productive in your work with the operating system. Whether you're a beginner or an experienced user, the shell provides a powerful tool for managing and automating tasks.

---------------------------

### [1. Shell, Basics](https://github.com/MathieuMorel62/holbertonschool-shell/tree/master/basics)
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), **without the help of Google:**
#### `General`

<details>
<summary>What does RTFM mean ?</summary>
<br>

>RTFM is an abbreviation for "Read The F***ing Manual." It's used to politely suggest to someone to consult the manual or documentation for a particular program or system before asking for help.
</details>
<details>
<summary>What is a Shebang</summary>
<br>

>A shebang is a special code in the first line of a script that specifies the interpreter to use for executing the script. It's represented as `#!` followed by the path to the interpreter, for example, `#!/bin/bash` specifies that the script should be run using the bash shell.
</details>
<details>
<summary>What is the shell</summary>
<br>

>The shell is a command-line interface that provides access to the underlying operating system. It allows users to perform tasks such as navigating the file system, managing files and directories, and running programs.
</details>
<details>
<summary>What is the difference between a terminal and a shell</summary>
<br>

>A terminal is a program that allows users to interact with the shell, while the shell is the command-line interface itself. The terminal provides a graphical interface for entering commands, while the shell is responsible for executing those commands.
</details>
<details>
<summary>What is the shell prompt</summary>
<br>

>The shell prompt is the symbol that indicates the shell is ready to receive commands. It typically shows the current directory and user information.
</details>
<details>
<summary>How to use the history (the basics)</summary>
<br>

>The shell maintains a history of previously executed commands. To view your command history, you can use the `history` command. To re-execute a previous command, you can use the `!` followed by the command number, for example, `!123` would execute the command with number 123 from the history. You can also use the up and down arrow keys to navigate the command history.
</details>
<details>
<summary>What do the commands or built-ins cd, pwd, ls do</summary>
<br>

>The `cd` (change directory) command is used to navigate the file system. For example, `cd /path/to/directory` changes the current directory to `/path/to/directory`. The `pwd` (print working directory) command displays the absolute path of the current working directory. The `ls` (list) command is used to list the contents of a directory. For example, `ls /path/to/directory` lists the contents of `/path/to/directory`.
</details>
<details>
<summary>How to navigate the filesystem</summary>
<br>

>To navigate the file system, you can use the `cd` command to change the current working directory and the `ls` command to list the contents of a directory. The `pwd` command can be used to display the current working directory.
</details>
<details>
<summary>What are the . and .. directories</summary>
<br>

>The `.` directory represents the current directory, while the `..` directory represents the parent directory. For example, cd `..` changes the current directory to the parent directory.
</details>
<details>
<summary>What is the working directory, how to print it and how to change it</summary>
<br>

>The working directory is the current directory that the shell is operating in. To display the working directory, you can use the `pwd` command. To change the working directory, you can use the `cd` command.
</details>
<details>
<summary>What is the root directory</summary>
<br>

>The root directory is the top-most directory in the file system hierarchy, represented by the `/` symbol. It contains all other directories and files on the system.
</details>
<details>
<summary>What is the home directory, and how to go there</summary>
<br>

>The home directory is the personal directory for a user, typically represented by the `~` symbol. For example, `cd ~` changes the current directory to the user's home directory.
</details>
<details>
<summary>What is the difference between the root directory and the home directory of the user root</summary>
<br>

>The root directory (`/`) is the top-most directory in the file system hierarchy, and is accessible by the superuser `root`. The home directory of the user `root` is `/root`, which is the personal directory for the `root` user.
</details>
<details>
<summary>What are the characteristics of hidden files and how to list them</summary>
<br>

>Hidden files are files that are not displayed by default in a directory listing. They are typically indicated by a `.` prefix in front of the file name. To list hidden files, you can use the `ls -a` command.
</details>
<details>
<summary>What does the command cd - do</summary>
<br>

>The `cd -` command changes the current directory to the previous working directory. This can be useful for quickly switching back and forth between two directories.
</details>
<details>
<summary>What do the commands ls, less, file do</summary>
<br>

>The `ls` command is used to list the files and directories in a directory. It stands for "list". The `less` command is used to display the contents of a file one page at a time. It is similar to the `more` command, but offers more features and is more commonly used. The `file` command is used to determine the type of a file. It can identify the format of a file, such as whether it is an executable file, a text file, or an image file, etc.
</details>
<details>
<summary>How do you use options and arguments with commands</summary>
<br>

>Options and arguments are used to modify the behavior of a command. An option starts with a dash (`-`) and is used to specify a particular behavior, while an argument is a value that is passed to the command to be used as input. For example, the `ls` command can be used with the `-l` option to display the files in a long format, or with the `-a` option to show hidden files.
</details>
<details>
<summary>Understand the ls long format and how to display it</summary>
<br>

>The long format of the `ls` command is used to display detailed information about the files and directories in a directory. It shows information such as the file's permissions, owner, group, size, date, and time of the last modification, etc. The long format is displayed using the `-l` option.
</details>

- [A Guided Tour](https://intranet.hbtn.io/rltoken/GznRkhU3QTWAWwDeZ-k9Pw)

<details>
<summary>What does the ln command do</summary>
<br>

>The `ln` command is used to create links between files. There are two types of links: symbolic links (also known as soft links) and hard links. A symbolic link is a reference to another file that can be used as if it were the original file, while a hard link is a second directory entry that points to the same data on disk as the original file.
</details>
<details>
<summary>What do you find in the most common/important directories</summary>
<br>

>Some of the most common and important directories in a Unix-like operating system include:

- `/` (root directory): The top-level directory of the file system.
- `/bin`: Contains binary executable files that are used by the system and the users.
- `/etc`: Contains configuration files for the system and applications.
- `/dev`: Contains special files that represent devices.
- `/home`: Contains the home directories for the users.
- `/lib`: Contains shared libraries used by the system and applications.
- `/tmp`: Contains temporary files that are created by the system and applications.
</details>
<details>
<summary>What is a symbolic link</summary>
<br>

>A symbolic link (also known as a soft link) is a reference to another file that can be used as if it were the original file. A symbolic link is similar to a shortcut in Windows. When you access a symbolic link, you are actually accessing the file that it points to. If the original file is deleted or moved, the symbolic link will become broken.
</details>
<details>
<summary>What is a hard link</summary>
<br>

>A hard link is a second directory entry that points to the same data on disk as the original file. When you access a hard link, you are accessing the same data on disk as the original file. If the original file is deleted, the hard link will continue to point to the data on disk and can still be used.
</details>
<details>
<summary>What is the difference between a hard link and a symbolic link</summary>
<br>

>The main difference between a hard link and a symbolic link is that a hard link points directly to the data on disk, while a symbolic link points to another file. When you access a hard link, you are accessing the same data on disk as the original file, while when you access a symbolic link
</details>
<details>
<summary>What do the commands cp, mv, rm, mkdir do</summary>
<br>

>`cp`: Copies files and directories. `mv`: Moves or renames files and directories. `rm`: Removes files and directories. `mkdir`: Creates a new directory.
</details>
<details>
<summary>What are wildcards and how do they work</summary>
<br>

>Wildcards are characters that can be used to match one or more files or directories. The most commonly used wildcards are `*` and `?`. The `*` wildcard matches any number of characters, while the `?` wildcard matches exactly one character.
</details>
<details>
<summary>How to use wildcards</summary>
<br>

>How to use wildcards: Wildcards can be used in combination with commands such as `ls`, `cp`, `mv`, and `rm` to match multiple files or directories. For example, `ls *` will list all files and directories in the current directory, while `rm *.txt` will remove all files with a .txt extension. The `*` and `?` characters can also be used to match specific patterns, such as `*.jpg` to match all files with a `.jpg` extension.
</details>
<details>
<summary>What do type, which, help, man commands do</summary>
<br>

>The `type` command in Unix-like systems is used to determine the type of command or a command's location (i.e., which executable file in the PATH will be executed). The `which` command is used to locate an executable file in the PATH. It can also be used to determine if a command is an alias, shell function, built-in command, or an external command. The `help` command provides information about built-in commands in shells like Bash. It is usually used for simple, brief information about the usage and syntax of a command. The `man` (manual) command provides access to the manual pages for Unix-like systems. The manual pages contain more detailed information about the commands and their options.
</details>
<details>
<summary>What are the different kinds of commands</summary>
<br>

>Different kinds of commands in Unix-like systems include:
- Built-in commands (e.g., `cd`, `pwd`)
- External commands (e.g., `ls`, `grep`)
- Aliases (user-defined shorthand for frequently used commands)
- Shell functions (user-defined commands executed in the current shell)
- System calls (functions executed by the kernel to perform specific system-level operations)
- Library functions (reusable code accessible to programs)
</details>
<details>
<summary>What is an alias</summary>
<br>

>An alias is a user-defined shorthand for a frequently used command. It can be used to create short, memorable command names for long or complex commands. For example, you could create an alias for the `ls -l` command as `ll`, so that you can simply type `ll` to get a long listing of files in the current directory.
</details>
<details>
<summary>When do you use the command help instead of man</summary>
<br>

>The `help` command is used when you need simple, brief information about the usage and syntax of a command. The `man` command is used when you need more detailed information about a command, including options and examples.
</details>
<details>
<summary>How to read a man page</summary>
<br>

>To read a man page, type the `man` command followed by the name of the command you're interested in. For example, `man ls` will display the manual page for the `ls` command. You can navigate the man page using the up and down arrow keys or the space bar. To exit the man page, type `q`.
</details>
<details>
<summary>What are man page sections</summary>
<br>

>The manual pages are divided into sections, which contain information about different aspects of the commands.
</details>
<details>
<summary>What are the section numbers for User commands, System calls and Library functions</summary>
<br>

>The standard section numbers for man pages are:

- 1: User commands
- 2: System calls
- 3: Library functions
- 4: Special files (e.g., device files)
- 5: File formats and conventions
- 6: Games and screensavers
- 7: Miscellanea
- 8: System management commands (administrator commands)
</details>
<details>
<summary>Common shortcuts for Bash</summary>
<br>

>Common shortcuts for the Bash shell include:

- `ctrl + a`: Move to the beginning of the line
- `ctrl + e`: Move to the end of the line
- `ctrl + u`: Clear the line before the cursor
- `ctrl + k`: Clear the line after the cursor
- `ctrl + r`: Search the command history
- `ctrl + l`: Clear the terminal screen
</details>
<details>
<summary>What does LTS mean ?</summary>
<br>

>LTS stands for Long-Term Support. In the context of software, it refers to a version of the software that is actively maintained and supported by the developers for a longer period of time, typically several years, compared to other versions. LTS releases are meant to be more stable and secure, and are often recommended for use in production environments.
</details>

---------------------------------

### [2. Shell, Permissions](https://github.com/MathieuMorel62/holbertonschool-shell/tree/master/permissions)
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), **without the help of Google:**
#### `General`

<details>
<summary>What do the commands chmod, sudo, su, chown, chgrp do</summary>
<br>

>`chmod`: This is the command used in Linux to change the permissions on a file or directory. `sudo`: This is the command used to run a command with administrative (root) privileges. When you run a command with sudo, the system prompts you for your password, and then executes the command with root privileges. `su`: This stands for "switch user" and allows you to switch to another user account, usually the root account. This can be used to gain administrative privileges on the system. `chown`: This stands for "change owner" and is used to change the owner of a file or directory. `chgrp`: This stands for "change group" and is used to change the group ownership of a file or directory.
</details>
<details>
<summary>Linux file permissions</summary>
<br>

>In Linux, file permissions are represented by a set of 10 characters that define the read, write, and execute permissions for the file's owner, group, and others.
</details>
<details>
<summary>How to represent each of the three sets of permissions (owner, group, and other) as a single digit</summary>
<br>

>Each set of permissions (owner, group, others) can be represented as a single digit using octal (base-8) notation. The digit is calculated based on the permissions set for each file. For example, if a file has read and write permissions for the owner and only read permission for group and others, the permission can be represented as 644 (rw-r--r--).
</details>
<details>
<summary>How to change permissions, owner and group of a file</summary>
<br>

>To change permissions, owner, or group of a file in Linux, you can use the `chmod`, `chown`, and `chgrp` commands. For example, to change the permissions on a file named "example.txt" to read and write for the owner and only read for group and others, you can run the following command: `chmod 644 example.txt`
</details>
<details>
<summary>Why can’t a normal user chown a file</summary>
<br>

>Only the root user or a user with root privileges (using `sudo`) can change the owner of a file. This is because changing the owner of a file has the potential to affect the security of the system and therefore is restricted to privileged users.
</details>
<details>
<summary>How to run a command with root privileges</summary>
<br>

> To run a command with root privileges, you can use the `sudo` command. For example, to run the `ls` command with root privileges, you can run the following command: `sudo ls`
</details>
<details>
<summary>How to change user ID or become superuser</summary>
<br>

>To change your user ID to become the superuser (root), you can use the `su` command. This requires that you know the root password. For example, to become the root user, you can run the following command: `su`.
</details>
<details>
<summary>How to create a user</summary>
<br>

>To create a user in Linux, you can use the `useradd` command. For example, to create a user named "newuser", you can run the following command: `sudo useradd newuser`
</details>
<details>
<summary>How to create a group</summary>
<br>

>To create a group in Linux, you can use the `groupadd` command. For example, to create a group named "newgroup", you can run the following command: `sudo groupadd newgroup`
</details>
<details>
<summary>How to print real and effective user and group IDs</summary>
<br>

>To print the real and effective user and group IDs, you can use the `id` command. The real user ID (UID) and group ID (GID) are the ones associated with the user that initially logged in to the system. The effective UID and GID are the ones used by the system to determine the permissions for a user's actions. For example, to print the real and effective UID and GID, you can run the following command: `id -u -g`
</details>
<details>
<summary>How to print the groups a user is in</summary>
<br>

>Printing the groups a user is in: To print the groups a user is in, you can use the `id` command with the `-Gn` option. For example, to print the groups for the current user, you can run the following command: `id -Gn`
</details>
<details>
<summary>How to print the effective userid</summary>
<br>

>To print the effective user ID (EUID), you can use the `id` command with the `-u` option. For example, to print the effective user ID for the current user, you can run the following command: `id -u`
</details>

--------------------------

### [3. Shell, I/O Redirections And Filters](https://github.com/MathieuMorel62/holbertonschool-shell/tree/master/io_redirections_and_filters)
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), **without the help of Google:**
#### `General`

<details>
<summary>What do the commands head, tail, find, wc, sort, uniq, grep, tr</summary>
<br>

>The different commands are:

- `head`: This command displays the first few lines of a file. By default, `head` displays the first 10 lines of a file, but you can specify a different number of lines using the `-n` option.
- `tail`: This command displays the last few lines of a file. By default, `tail` displays the last 10 lines of a file, but you can specify a different number of lines using the `-n` option.
- `find`: This command is used to search for files and directories in a specified location. You can specify criteria for the search, such as the file name, type, size, or modification time.
- `wc`: This command stands for "word count" and is used to count the number of lines, words, and characters in a file.
- `sort`: This command is used to sort the lines of a file. By default, the `sort` is performed in lexicographic order, but you can specify other criteria using options such as `-n` (numeric sort), `-r` (reverse sort), and `-k` (sort based on a specific field).
- `uniq`: This command is used to remove duplicate lines from a file.
- `grep`: This command is used to search for patterns in a file. `grep` searches for a specified regular expression in the input and displays all lines that match the pattern.
- `tr`: This command stands for "translate" and is used to translate or delete characters in a file.
</details>
<details>
<summary>How to redirect standard output to a file</summary>
<br>

>You can redirect the standard output of a command to a file using the `>` operator. For example, to redirect the output of the `ls` command to a file named "list.txt", you can run the following command: `ls > list.txt`
</details>
<details>
<summary>How to get standard input from a file instead of the keyboard</summary>
<br>

>You can get the standard input for a command from a file instead of the keyboard using the `<` operator. For example, to run the `wc` command on the contents of a file named "example.txt", you can run the following command: `wc < example.txt`
</details>
<details>
<summary>How to send the output from one program to the input of another program</summary>
<br>

>You can send the output from one program to the input of another program using a pipe (`|`). The pipe takes the standard output of the command on the left and uses it as the standard input for the command on the right. For example, to sort the contents of a file named "example.txt" and display the sorted contents, you can run the following command: `sort < example.txt`
</details>
<details>
<summary>How to combine commands and filters with redirections</summary>
<br>

>You can combine multiple commands and filters to perform more complex operations on data. For example, to sort the contents of a file named "example.txt", remove duplicate lines, and display the unique, sorted contents, you can run the following command: `sort < example.txt | uniq`
</details>
<details>
<summary>What are special characters</summary>
<br>

>In the context of the shell, special characters are characters that have a special meaning and are used to perform certain operations.
</details>
<details>
<summary>Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde and how and when to use them</summary>
<br>

>The different characters are:

- `White spaces`: White spaces are characters that represent spaces, tabs, and line breaks. They are used to separate arguments in a shell command and can be used to separate items in a list.
- `Single quotes (')`: Single quotes are used to specify a literal string. When a string is enclosed in single quotes, all characters within the quotes are treated as literal characters, and no special meaning is assigned to any of the characters. For example: `'hello world'`
- `Double quotes (")`: Double quotes are similar to single quotes, but they allow for the expansion of variables. For example: `"hello $user"`
- `Backslash ()`: The backslash is used to escape special characters. For example, to include a single quote within a string enclosed in single quotes, you can use a backslash to escape the single quote: `'hello\' world'`
- `Comment (#)`: The comment character is used to indicate that the rest of the line should be ignored. Everything after the `#` symbol is considered a comment and is not executed as part of the command.
- `Pipe (|)`: The pipe is used to redirect the output of one command to the input of another command. The pipe takes the standard output of the command on the left and uses it as the standard input for the command on the right. For example: `ls | grep '.txt'`
- `Command separator (;)`: The command separator is used to separate multiple commands on the same line. When the command separator is used, each command is executed in sequence, and the results of one command are used as the input for the next command. For example: `ls; pwd`
- `Tilde (~)`: The tilde is used as a shortcut to refer to the home directory of the current user. For example: `cd ~`
</details>
<details>
<summary>How to display a line of text</summary>
<br>

>To display a line of text, you can use the `echo` command. For example, to display the text "Hello, World!", you would run the following command: `echo "Hello, World!"`
</details>
<details>
<summary>How to concatenate files and print on the standard output</summary>
<br>

>To concatenate files and print the result on the standard output, you can use the `cat` command. For example, to concatenate two files `file1.txt` and `file2.txt` and display the result on the standard output, you would run the following command: `cat file1.txt file2.txt`
</details>
<details>
<summary>How to reverse a string</summary>
<br>

>To reverse a string, you can use the `rev` command. For example, to reverse the string "Hello, World!", you would run the following command: `echo "Hello, World!" | rev`
</details>
<details>
<summary>How to remove sections from each line of files</summary>
<br>

>To remove sections from each line of files, you can use the `cut` command. The `cut` command is used to extract sections of text from a file or input stream. For example, to extract the first 5 characters from each line of a file `file.txt`, you would run the following command: `cut -c 1-5 file.txt`
</details>
<details>
<summary>What is the /etc/passwd file and what is its format</summary>
<br>

>The `/etc/passwd` file is a system file that contains information about users on a Unix-like system. The file has the following format: `username:password:userID:groupID:user info:home directory:command/shell`
</details>
<details>
<summary>What is the /etc/shadow file and what is its format</summary>
<br>

>The `/etc/shadow` file is a system file that contains encrypted passwords for user accounts on a Unix-like system. The file has the following format: `username:password:last password change:minimum password age:maximum password age:password warning period:password inactivity period:account expiration`.
</details>

--------------------------------

### [4. Shell, Init Files, Variables And Expansions](https://github.com/MathieuMorel62/holbertonschool-shell/tree/master/init_files_variables_and_expansions)
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), **without the help of Google:**
#### `General`

<details>
<summary>What happens when you type $ ls -l *.txt</summary>
<br>

>When you type `ls -l *.txt`, the shell expands the `*.txt` wildcard to match all files in the current directory with a `.txt` extension and then passes the list of matched filenames to the `ls` command. The `ls` command then displays a long listing of information about each of the matched files, including the file permissions, owner, group, size, and timestamps.
</details>
<details>
<summary>What are the /etc/profile file and the /etc/profile.d directory</summary>
<br>

>The `/etc/profile` file is a system-wide shell configuration file that is read by the shell when a user logs in to the system. The file contains global settings and configurations that are applied to all users on the system. The `/etc/profile.d` directory is a collection of shell script files that are executed when a user logs in to the system. The scripts in this directory are typically used to set up specific shell environment variables, configure shell options, or define aliases for all users on the system.
</details>
<details>
<summary>What is the ~/.bashrc file</summary>
<br>

>The `~/.bashrc` file is a per-user shell configuration file that is read by the shell when a user starts a new shell session. The file contains settings and configurations that are specific to a single user and are applied each time the user starts a new shell session.
</details>
<details>
<summary>What is the difference between a local and a global variable</summary>
<br>

>A local variable is a variable that is declared within a shell script or function and is only accessible within the scope of that script or function. A global variable, on the other hand, is a variable that is declared outside of any scripts or functions and is accessible from anywhere within the shell environment.
</details>
<details>
<summary>What is a reserved variable</summary>
<br>

>A reserved variable is a variable that has a special meaning in the shell and is used for specific purposes, such as storing the exit status of a command or tracking the current directory. Some examples of reserved variables include `$?`, `$0`, and `$PWD`.
</details>
<details>
<summary>How to create, update and delete shell variables</summary>
<br>

>To create a shell variable, you can assign a value to a variable name using the following syntax: `variable_name=value`. To update the value of an existing variable, you can simply assign a new value to the variable using the same syntax. To delete a shell variable, you can use the `unset` command. For example, to delete the variable `variable_name`, you would run the following command: `unset variable_name`.
</details>
<details>
<summary>What are the roles of the following reserved variables: HOME, PATH, PS1</summary>
<br>

>Roles of the reserved variables:

- `HOME`: The `HOME` variable stores the path to the home directory of the current user.
- `PATH`: The `PATH` variable is a list of directories that the shell searches for executable files.
- `PS1`: The `PS1` variable is the primary prompt string and is used to display the command prompt in the shell.
</details>
<details>
<summary>What are special parameters</summary>
<br>

>Special parameters are reserved variables that are used to store information about the current shell environment and the status of previously executed commands. Some examples of special parameters include `$1`, `$2`, and `$#`, which are used to access the arguments passed to a shell script, and `$?`, which stores the exit status of the last executed command.
</details>
<details>
<summary>What is the special parameter $? ?</summary>
<br>

>The `$?` special parameter is a reserved variable that stores the exit status of the last executed command and is used to determine if the command was successful or not. A value of 0 indicates that the command was successful, while a non-zero value indicates that the command failed
</details>
<details>
<summary>What is expansion and how to use them</summary>
<br>

> In shell scripting, expansion is a process of replacing a specific pattern with a value or string. There are several types of expansions in shell scripting, such as parameter expansion, command substitution, and arithmetic expansion.
</details>
<details>
<summary>What is the difference between single and double quotes and how to use them properly</summary>
<br>

>Single vs Double Quotes: In shell scripting, there are two types of quotes: single quotes (`'`) and double quotes (`"`). Single quotes preserve the literal value of each character within the quotes, while double quotes allow for parameter and command expansion. For example:

```shell
$ echo 'This is a string'
This is a string
$ echo "This is a string with a parameter expansion: $SHELL"
This is a string with a parameter expansion: /bin/bash
```
</details>
<details>
<summary>How to do command substitution with $() and backticks</summary>
<br>

>Command substitution allows the output of a command to be used as an argument to another command. There are two ways to perform command substitution: with `$()` and backticks (`). For example:

```shell
$ echo Today is $(date)
Today is Mon Feb 11 21:23:48 UTC 2023
$ echo Today is `date`
Today is Mon Feb 11 21:23:48 UTC 2023
```
</details>
<details>
<summary>How to perform arithmetic operations with the shell</summary>
<br>

>In shell scripting, you can perform arithmetic operations using the `$(( ))` syntax. For example:

```shell
$ echo $((2 + 2))
4
$ echo $((2 * 2))
4
$ echo $((10 / 2))
5
```
</details>
<details>
<summary>How to create an alias</summary>
<br>

>An alias is a shorthand way to refer to a command or set of commands. To create an alias in the shell, use the `alias` command followed by the desired alias name and the command or set of commands it should represent. For example:

```shell
$ alias ll='ls -lh'
```
</details>
<details>
<summary>How to list aliases</summary>
<br>

>To list the defined aliases in the current shell, use the `alias` command without any arguments:

```shell
$ alias
alias ll='ls -lh'
```
</details>
<details>
<summary>How to temporarily disable an alias</summary>
<br>

>To temporarily disable an alias, you can unalias it using the `unalias` command. For example:

```shell
$ unalias ll
$ ll
-bash: ll: command not found
```
</details>
<details>
<summary>How to execute commands from a file in the current shell</summary>
<br>

>To execute commands from a file in the current shell, use the `source` command followed by the file name. The `source` command reads the file line by line and executes each line as a separate command in the current shell. For example:

```bash
$ cat commands.sh
#!/bin/bash
echo "This is a test"
$ source commands.sh
This is a test
```
</details>

----------------------------------

## Author

- Mathieu Morel
