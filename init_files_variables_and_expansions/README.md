# SHELL, INIT FILES, VARIABLES AND EXPANSIONS

![img](https://miro.medium.com/max/1400/1*Yln1pgshMWJsX7p4HxTzAA.png)

## RESOURCES

### Read or watch :

- [Expansions](https://intranet.hbtn.io/rltoken/qvjamZX_aoZmdZOiEapxzw)
- [Shell Arithmetic](https://intranet.hbtn.io/rltoken/CuAnsjJ9mg_y-zBVwmn7mg)
- [Variables](https://intranet.hbtn.io/rltoken/vjgJv9-2mvkhoMT05Mk-VA)
- [Shell Initialization Files](https://intranet.hbtn.io/rltoken/0DxDIIG_UpoM7cKGhsuVWw)
- [The Alias Command](https://intranet.hbtn.io/rltoken/vOCzCs3YAUxGZlfD4PTeeg)
- [Technical Writing](https://intranet.hbtn.io/rltoken/-f0eRmOjXoyySeqW6xvc7Q)

--------------------------

# TASKS


### [0. < o >](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/0-alias)

Create a script that creates an alias.

  - Name: `ls`
  - Value: `rm *`
  
<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ ls
0-alias  file1  file2
julien@ubuntu:/tmp/0x03$ source ./0-alias 
julien@ubuntu:/tmp/0x03$ ls
julien@ubuntu:/tmp/0x03$ \ls
julien@ubuntu:/tmp/0x03$ 
```
</details>

----------------------------------

### [1. Hello You](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/1-hello_you)

Create a script that prints `hello user`, where user is the current Linux user.

<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ id
uid=1000(julien) gid=1000(julien) groups=1000(julien),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),113(lpadmin),128(sambashare)
julien@ubuntu:/tmp/0x03$ ./1-hello_you 
hello julien
julien@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [2. The Path To Success Is To Take Massive, Determinated Action](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/2-path)

Add `/action` to the `PATH`. `/action` should be the last directory the shell looks into when looking for a program.

<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ source ./2-path 
julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/action
julien@ubuntu:/tmp/0x03$ 
```
</details>

-------------------------------

### [3. If The Path Be Beautiful, Let Us Not Ask Where It Leads](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/3-paths)

Create a script that counts the number of directories in the `PATH`.

<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ . ./3-paths 
11
julien@ubuntu:/tmp/0x03$ PATH=/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:::::/hello
julien@ubuntu:/tmp/0x03$ . ./3-paths 
12
julien@ubuntu:/tmp/0x03$ 
```
</details>

------------------------------

### [4. Global Variables](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/4-global_variables)

Create a script that lists environment variables.

<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ source ./4-global_variables
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
julien@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [5. Local Variables](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/5-local_variables)

Create a script that lists all local variables and environment variables, and functions.

<details>
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ . ./5-local_variables
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
julien@ubuntu:/tmp/0x03$ 
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
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~$ export TRUEKNOWLEDGE=1209
julien@production-503e7013:~$ ./8-true_knowledge | cat -e
1337$
julien@production-503e7013:~$
```
</details>

-----------------------------

### [9. Divide And Rule]( https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/9-divide_and_rule)

Write a script that prints the result of `POWER` divided by `DIVIDE`, followed by a new line.

  - `POWER` and `DIVIDE` are environment variables
  
<details>
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~$ export POWER=42784
julien@production-503e7013:~$ export DIVIDE=32
julien@production-503e7013:~$ ./9-divide_and_rule | cat -e
1337$
julien@production-503e7013:~$
```
</details>

------------------------------

### [10. Love Is Anterior To Life, Posterior To Death, Initial Of Creation, And The Exponent Of Breath](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/10-love_exponent_breath)

Write a script that displays the result of `BREATH` to the power `LOVE`

  - `BREATH` and `LOVE` are environment variables
  - The script should display the result, followed by a new line

<details>
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~/$ export BREATH=4
julien@production-503e7013:~/$ export LOVE=3
julien@production-503e7013:~/$ ./10-love_exponent_breath
64
julien@production-503e7013:~/$
```
</details>

------------------------------

### [11. There Are 10 Types Of People In The World -- Those Who Understand Binary, And Those Who Don't](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/11-binary_to_decimal)

Write a script that converts a number from base 2 to base 10.

  - The number in base 2 is stored in the environment variable `BINARY`
  - The script should display the number in base 10, followed by a new line


<details>
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~/$ export BINARY=10100111001
julien@production-503e7013:~/$ ./11-binary_to_decimal
1337
julien@production-503e7013:~/$
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
<summary>Click to see the example</summary>
<br>

```
julien@ubuntu:/tmp/0x03$ echo $((26 ** 2 -1))
675
julien@ubuntu:/tmp/0x03$ ./12-combinations | wc -l
675
julien@ubuntu:/tmp/0x03$ 
julien@ubuntu:/tmp/0x03$ ./12-combinations | tail -303 | head -10
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
julien@ubuntu:/tmp/0x03$ 
```
</details>

---------------------------

### [13. Floats](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/13-print_float)

Write a script that prints a number with two decimal places, followed by a new line.

The number will be stored in the environment variable `NUM`.

<details>
<summary>Click to see the example</summary>
<br>

```
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
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~/$ export DECIMAL=16
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal
10
julien@production-503e7013:~/$ export DECIMAL=1337
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
539$
julien@production-503e7013:~/$ export DECIMAL=15
julien@production-503e7013:~/$ ./14-decimal_to_hexadecimal | cat -e
f$
julien@production-503e7013:~/$
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
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~/shell/fun_with_the_shell$ cat quote
"Everyone is a proponent of strong encryption."
- Dorothy E. Denning
julien@production-503e7013:~/shell/fun_with_the_shell$ ./15-rot13 < quote
"Rirelbar vf n cebcbarag bs fgebat rapelcgvba."
- Qbebgul R. Qraavat
julien@production-503e7013:~/shell/fun_with_the_shell$
```
</details>

--------------------------

### [17. The Eggs Of The Brood Need To Be An Odd Number](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/init_files_variables_and_expansions/16-odd)

Write a script that prints every other line from the input, starting with the first line.

<details>
<summary>Click to see the example</summary>
<br>

```
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
<summary>Click to see the example</summary>
<br>

```
julien@production-503e7013:~$ export WATER="ewwatratewa"
julien@production-503e7013:~$ export STIR="ti.itirtrtr"
julien@production-503e7013:~$ ./17-water_and_stir
shtbeolhc
julien@production-503e7013:~$
```
</details>

-----------------------------------
