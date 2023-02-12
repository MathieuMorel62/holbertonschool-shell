# <p align="center">SHELL, INIT FILES, VARIABLES AND EXPANSIONS</p>

<img src="https://miro.medium.com/max/1400/1*Yln1pgshMWJsX7p4HxTzAA.png" width="100%">

## Description
### Introduction to Shell, Init Files, Variables and Expansions
  
The shell is a powerful tool in Unix-based operating systems that allows you to interact with the underlying system by providing a command-line interface. It is a program that reads and executes commands, which can be typed directly into the terminal or read from a script file.
  
There are many different shell implementations available, with the most popular being the Bourne-Again SHell (Bash).

### Init Files

When a shell is started, it reads and executes commands from a series of configuration files, also known as "init files". These files contain environment variables, functions and commands that are executed every time you start a new shell session. The most commonly used init files are:
  
- `~/.bashrc`: This file is specific to the Bash shell and is executed every time you start a new interactive shell session.
- `~/.bash_profile`: This file is also specific to the Bash shell and is executed when you log in to your system.
- `/etc/profile`: This file contains system-wide environment settings and is executed for all users when they log in to the system.

### Variables
  
Variables in the shell are used to store and manipulate data. They are an important tool for managing your environment and can be used to store values such as file paths, user information, and other configuration settings.
  
To define a variable, you simply use the following syntax:

```bash
variable_name=value
```

For example:

```bash
name=John
```

To access the value of a variable, you use a dollar sign $ followed by the name of the variable, like this:

```bash
echo $name
```

This will print the value of the `name` variable, which in this case is "John".

### Expansions

Expansions are a way to substitute the value of a variable or perform operations on it. There are several types of expansions in the shell, including:

- Command substitution: This allows you to run a command and substitute its output in place of the expansion. You can use either backticks (\`) or `$( )` to perform command substitution.
- Arithmetic expansion: This allows you to perform arithmetic operations on variables. You can use the `$(( ))` syntax to perform arithmetic expansions.
- Pathname expansion: This allows you to expand the value of a variable to match a file path pattern. The shell uses the `*`, `?`, and `[]` characters to perform pathname expansion.
- Brace expansion: This allows you to generate a sequence of values by specifying a range of values within curly braces `{}`.
  
Expansions are an important tool for automating tasks and making your scripts more efficient. By using expansions, you can write scripts that are more dynamic and flexible, and that can adapt to changing conditions without the need for manual intervention.

### Conclusion

In conclusion, the shell is a powerful tool that provides a command-line interface to interact with your operating system. By using init files, variables, and expansions, you can manage your environment and automate tasks, making your work more efficient and less prone to error. Whether you are an experienced system administrator or just starting out, understanding these concepts is essential to getting the most out of the shell.

## Resources
### Read or Watch :

- [Expansions](https://intranet.hbtn.io/rltoken/qvjamZX_aoZmdZOiEapxzw)
- [Shell Arithmetic](https://intranet.hbtn.io/rltoken/CuAnsjJ9mg_y-zBVwmn7mg)
- [Variables](https://intranet.hbtn.io/rltoken/vjgJv9-2mvkhoMT05Mk-VA)
- [Shell Initialization Files](https://intranet.hbtn.io/rltoken/0DxDIIG_UpoM7cKGhsuVWw)
- [The Alias Command](https://intranet.hbtn.io/rltoken/vOCzCs3YAUxGZlfD4PTeeg)
- [Technical Writing](https://intranet.hbtn.io/rltoken/-f0eRmOjXoyySeqW6xvc7Q)

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All your scripts will be tested on Ubuntu 20.04 LTS
- All your scripts should be exactly two lines long (`$ wc -l` file should print 2)
- All your files should end with a new line ([why?](http://unix.stackexchange.com/questions/18743/whats-the-point-in-adding-a-new-line-to-the-end-of-a-file/18789))
- The first line of all your files should be exactly `#!/bin/bash`
- A `README.md` file, at the root of the folder of the project, describing what each script is doing
- You are not allowed to use `&&`, `||` or `;`
- You are not allowed to use `bc`, `sed` or `awk`
- All your files must be executable

--------------------------

# TASKS

### [0. < o >](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/0-alias)

Create a script that creates an alias.
- Name: `ls`
- Value: `rm *`
  
<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ ls
0-alias  file1  file2
mathieu:/tmp/0x03$ source ./0-alias 
mathieu@ubuntu:/tmp/0x03$ ls
mathieu@ubuntu:/tmp/0x03$ \ls
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

----------------------------------

### [1. Hello You](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/1-hello_you)

Create a script that prints `hello user`, where user is the current Linux user.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ id
uid=1000(mathieu) gid=1000(mathieu) groups=1000(mathieu),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),113(lpadmin),128(sambashare)
mathieu@ubuntu:/tmp/0x03$ ./1-hello_you 
hello mathieu
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [2. The Path To Success Is To Take Massive, Determinated Action](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/2-path)

Add `/action` to the `PATH`. `/action` should be the last directory the shell looks into when looking for a program.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ echo $PATH
/home/mathieu/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
mathieu@ubuntu:/tmp/0x03$ source ./2-path 
mathieu@ubuntu:/tmp/0x03$ echo $PATH
/home/mathieu/bin:/home/mathieu/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/action
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

-------------------------------

### [3. If The Path Be Beautiful, Let Us Not Ask Where It Leads](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/3-paths)

Create a script that counts the number of directories in the `PATH`.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ echo $PATH
/home/mathieu/bin:/home/mathieu/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
mathieu@ubuntu:/tmp/0x03$ . ./3-paths 
11
mathieu@ubuntu:/tmp/0x03$ PATH=/home/mathieu/bin:/home/mathieu/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:::::/hello
mathieu@ubuntu:/tmp/0x03$ . ./3-paths 
12
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

------------------------------

### [4. Global Variables](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/4-global_variables)

Create a script that lists environment variables.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ source ./4-global_variables
CC=gcc
CDPATH=.:~:/usr/local:/usr:/
CFLAGS=-O2 -fomit-frame-pointer
COLORTERM=gnome-terminal
CXXFLAGS=-O2 -fomit-frame-pointer
DISPLAY=:0
DOMAIN=hq.garrels.be
e=
TOR=vi
FCEDIT=vi
FIGNORE=.o:~
G_BROKEN_FILENAMES=1
GDK_USE_XFT=1
GDMSESSION=Default
GNOME_DESKTOP_SESSION_ID=Default
GTK_RC_FILES=/etc/gtk/gtkrc:/nethome/franky/.gtkrc-1.2-gnome2
GWMCOLOR=darkgreen
GWMTERM=xterm
HISTFILESIZE=5000
history_control=ignoredups
HISTSIZE=2000
HOME=/nethome/franky
HOSTNAME=octarine.hq.garrels.be
INPUTRC=/etc/inputrc
IRCNAME=franky
JAVA_HOME=/usr/java/j2sdk1.4.0
LANG=en_US
LDFLAGS=-s
LD_LIBRARY_PATH=/usr/lib/mozilla:/usr/lib/mozilla/plugins
LESSCHARSET=latin1
LESS=-edfMQ
LESSOPEN=|/usr/bin/lesspipe.sh %s
LEX=flex
LOCAL_MACHINE=octarine
LOGNAME=franky
[...]
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [5. Local Variables](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/5-local_variables)

Create a script that lists all local variables and environment variables, and functions.

<details>
<summary>Click to see the example</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ . ./5-local_variables
BASH=/bin/bash
BASHOPTS=checkwinsize:cmdhist:complete_fullquote:expand_aliases:extglob:extquote:force_fignore:histappend:interactive_comments:progcomp:promptvars:sourcepath
BASH_ALIASES=()
BASH_ARGC=()
BASH_ARGV=()
BASH_CMDS=()
BASH_COMPLETION_COMPAT_DIR=/etc/bash_completion.d
BASH_LINENO=()
BASH_REMATCH=()
BASH_SOURCE=()
BASH_VERSINFO=([0]="4" [1]="3" [2]="46" [3]="1" [4]="release" [5]="x86_64-pc-linux-gnu")
BASH_VERSION='4.3.46(1)-release'
CLUTTER_IM_MODULE=xim
COLUMNS=133
COMPIZ_CONFIG_PROFILE=ubuntu
COMP_WORDBREAKS=$' \t\n"\'><=;|&(:'
DBUS_SESSION_BUS_ADDRESS=unix:abstract=/tmp/dbus-Fg27Lr20bq
DEFAULTS_PATH=/usr/share/gconf/ubuntu.default.path
DESKTOP_SESSION=ubuntu
[...]
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

------------------------------

### [6. Local Variables](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/6-create_local_variable)

Create a script that creates a new local variable.
- Name: `BEST`
- Value: `School`

------------------------------

### [7. Global Variable](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/7-create_global_variable)

Create a script that creates a new global variable.
- Name: `BEST`
- Value: `School`

-----------------------------

### [8. Every Addition To True Knowledge Is An Addition To Human Power](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/8-true_knowledge)

Write a script that prints the result of the addition of 128 with the value stored in the environment variable `TRUEKNOWLEDGE`, followed by a new line.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~$ export TRUEKNOWLEDGE=1209
mathieu@production-503e7013:~$ ./8-true_knowledge | cat -e
1337$
mathieu@production-503e7013:~$
```
</details>

-----------------------------

### [9. Divide And Rule]( https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/9-divide_and_rule)

Write a script that prints the result of `POWER` divided by `DIVIDE`, followed by a new line.
- `POWER` and `DIVIDE` are environment variables
  
<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~$ export POWER=42784
mathieu@production-503e7013:~$ export DIVIDE=32
mathieu@production-503e7013:~$ ./9-divide_and_rule | cat -e
1337$
mathieu@production-503e7013:~$
```
</details>

------------------------------

### [10. Love Is Anterior To Life, Posterior To Death, Initial Of Creation, And The Exponent Of Breath](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/10-love_exponent_breath)

Write a script that displays the result of `BREATH` to the power `LOVE`
- `BREATH` and `LOVE` are environment variables
- The script should display the result, followed by a new line

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~/$ export BREATH=4
mathieu@production-503e7013:~/$ export LOVE=3
mathieu@production-503e7013:~/$ ./10-love_exponent_breath
64
mathieu@production-503e7013:~/$
```
</details>

------------------------------

#### [11. There Are 10 Types Of People In The World -- Those Who Understand Binary, And Those Who Don't](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/11-binary_to_decimal)

Write a script that converts a number from base 2 to base 10.
- The number in base 2 is stored in the environment variable `BINARY`
- The script should display the number in base 10, followed by a new line

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~/$ export BINARY=10100111001
mathieu@production-503e7013:~/$ ./11-binary_to_decimal
1337
mathieu@production-503e7013:~/$
```
</details>

-----------------------

### [12. Combination](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/12-combinations)

Create a script that prints all possible combinations of two letters, except `oo`.
- Letters are lower cases, from `a` to `z`
- One combination per line
- The output should be alpha ordered, starting with `aa`
- Do not print `oo`
- Your script file should contain maximum 64 characters

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@ubuntu:/tmp/0x03$ echo $((26 ** 2 -1))
675
mathieu@ubuntu:/tmp/0x03$ ./12-combinations | wc -l
675
mathieu@ubuntu:/tmp/0x03$ 
mathieu@ubuntu:/tmp/0x03$ ./12-combinations | tail -303 | head -10
oi
oj
ok
ol
om
on
op
oq
or
os
mathieu@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [13. Floats](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/13-print_float)

Write a script that prints a number with two decimal places, followed by a new line.

The number will be stored in the environment variable `NUM`.

<details>
<summary>File Test</summary>
<br>

```c++
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=0
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
0.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=98
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
98.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=3.14159265359
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
3.14
ubuntu@ip-172-31-63-244:~/0x03$
```
</details>

-------------------------

### [14. Decimal To Hexadecimal](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/14-decimal_to_hexadecimal)

Write a script that converts a number from base 10 to base 16.
- The number in base 10 is stored in the environment variable `DECIMAL`
- The script should display the number in base 16, followed by a new line

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~/$ export DECIMAL=16
mathieu@production-503e7013:~/$ ./14-decimal_to_hexadecimal
10
mathieu@production-503e7013:~/$ export DECIMAL=1337
mathieu@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
539$
mathieu@production-503e7013:~/$ export DECIMAL=15
mathieu@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
f$
mathieu@production-503e7013:~/$
```
</details>

---------------------------

### [15. What Happens When You Type LS*.C](https://medium.com/@mormth/what-happens-when-you-type-ls-c-in-the-terminal-d64519ca1d63)

Write a blog post describing step by step what happens when you type `ls *.c` and hit Enter in your shell. Try to explain every step you know of, and give examples. A total beginner should understand what you have written.
- Have at least one picture, at the top of the blog post
- Publish your blog post on Medium or LinkedIn
- Share your blog post at least on LinkedIn
- Write professionally and intelligibly
- Please, remember that these blogs must be written in English to further your technical ability in a variety of settings

When done, please add all urls below (blog post, LinkedIn post, etc.)

--------------------------

### [16. Everyone Is a Proponent Of Strong Encryption](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/15-rot13)

Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII.

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~/shell/fun_with_the_shell$ cat quote
"Everyone is a proponent of strong encryption."
- Dorothy E. Denning
mathieu@production-503e7013:~/shell/fun_with_the_shell$ ./15-rot13 < quote
"Rirelbar vf n cebcbarag bs fgebat rapelcgvba."
- Qbebgul R. Qraavat
mathieu@production-503e7013:~/shell/fun_with_the_shell$
```
</details>

--------------------------

### [17. The Eggs Of The Brood Need To Be An Odd Number](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/16-odd)

Write a script that prints every other line from the input, starting with the first line.

<details>
<summary>File Test</summary>
<br>

```c++
ubuntu@ip-172-31-63-244:/$ \ls -1
bin
boot
dev
etc
home
initrd.img
lib
lib32
lib64
libx32
lost+found
media
mnt
opt
proc
root
run
sbin
srv
sys
t
#t#
t~
tmp
usr
var
vmlinuz
whoareyou
ubuntu@ip-172-31-63-244:/$ \ls -1 | ./c-odd
bin
dev
home
lib
lib64
lost+found
mnt
proc
run
srv
t
t~
usr
vmlinuz
ubuntu@ip-172-31-63-244:/$
```
</details>

---------------------------

### [18. I'm An Instants Star. Just Add Water And Stir](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/17-water_and_stir)

Write a shell script that adds the two numbers stored in the environment variables `WATER` and `STIR` and prints the result.
- `WATER` is in base `water`
- `STIR` is in base `stir`.
- The result should be in base `bestchol`

<details>
<summary>File Test</summary>
<br>

```c++
mathieu@production-503e7013:~$ export WATER="ewwatratewa"
mathieu@production-503e7013:~$ export STIR="ti.itirtrtr"
mathieu@production-503e7013:~$ ./17-water_and_stir
shtbeolhc
mathieu@production-503e7013:~$
```
</details>

-----------------------------------

## Author

- Mathieu Morel
