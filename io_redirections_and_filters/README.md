# SHELL, I/O REDIRECTIONS AND FILTERS

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--NsAzIo2o--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/af2cde9k5712330xy457.png)

## RESOURCES

### Read or watch:

- [Shell, I/O Redirection](https://intranet.hbtn.io/rltoken/dJRc-mwT3vNw7SCWZNlGcg)

- [Special Characters](https://intranet.hbtn.io/rltoken/k2EzFVxAXrpfJMvl8-1ukQ)

--------------------------

# TASKS


### [0. Hello World](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/0-hello_world)

Write a script that prints “Hello, World”, followed by a new line to the standard output.

--------------------------

### [1. Confused Smiley](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/1-confused_smiley)

Write a script that displays a confused smiley "(Ôo)'.

------------------------

### [2. Let's Display a File](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/2-hellofile)

Display the content of the /etc/passwd file.

------------------------

### [3. What About 2 ?](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/3-twofiles)

Display the content of /etc/passwd and /etc/hosts

-----------------------

### [4. Last Lines Of a File](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/4-lastlines)

Display the last 10 lines of /etc/passwd

-----------------------

### [5. I'd Prefer The First Ones Actually](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/5-firstlines)

Display the first 10 lines of /etc/passwd

-------------------------

### [6. Line #2](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/6-third_line)

Write a script that displays the third line of the file iacta.

The file iacta will be in the working directory

  - You’re not allowed to use sed

--------------------------

### [7. It Is a Good File That Cuts Iron Without Making a Noise](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/7-file)

Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.

---------------------------

### [8. Save Current State Of Directory](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/8-cwd_state)

Write a script that writes into the file ls_cwd_content the result of the command ls -la. 

If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.

--------------------------------

### [9. Duplicate Last Line](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/9-duplicate_last_line)

Write a script that duplicates the last line of the file iacta

  - The file iacta will be in the working directory

---------------------------------

### [10. No More Javascript](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/10-no_more_js)

Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.

----------------------------

### [11. Don't Just Count Your Directories, Make Your Directories Count](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/11-directories)

Write a script that counts the number of directories and sub-directories in the current directory.

  - The current and parent directories should not be taken into account
  - Hidden directories should be counted

----------------------------

### [12. What's New](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/12-newest_files)

Create a script that displays the 10 newest files in the current directory.

Requirements :

  - One file per line
  - Sorted from the newest to the oldest

------------------------------

### [13. Being Unique Is Better Than Being Perfect](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/13-unique)

Create a script that takes a list of words as input and prints only words that appear exactly once.

  - Input format: One line, one word
  - Output format: One line, one word
  - Words should be sorted

----------------------------

### [14. It Must Be In That File](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/14-findthatword)

Display lines containing the pattern “root” from the file /etc/passwd

----------------------

### [15. Count That Word](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/15-countthatword)

Display the number of lines that contain the pattern “bin” in the file /etc/passwd

---------------------------

### [16. What's Next ?](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/16-whatsnext)

Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

--------------------------------

### [17. I Hate Bins](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/17-hidethisword)

Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.

--------------------------------

### [18. Letters Only Please](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/18-letteronly)

Display all lines of the file /etc/ssh/sshd_config starting with a letter.

  - include capital letters as well

---------------------------

### [19. A To Z](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/19-AZ)

Replace all characters A and c from input to Z and e respectively.

----------------------------

### [20. Without C, You Would Live In Hiago](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/20-hiago)

Create a script that removes all letters c and C from input.

---------------------------

### [21. Esrever](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/21-reverse)

Write a script that reverse its input.

----------------------------

### [22. Dj Cut Killer](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/22-users_and_homes)

Write a script that displays all users and their home directories, sorted by users.

  - Based on the the /etc/passwd file

------------------------------

### [23. Empty Casks Make The Most Noise](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/23-empty_casks)

Write a command that finds all empty files and directories in the current directory and all sub-directories.

  - Only the names of the files and directories should be displayed (not the entire path)
  - Hidden files should be listed
  - One file name per line
  - The listing should end with a new line
  - You are not allowed to use basename, grep, egrep, fgrep or rgrep

------------------------------

### [24. A Gif Is Worth Ten Thousand Words](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/24-gifs)

Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories.

  - Hidden files should be listed
  - Only regular files (not directories) should be listed
  - The names of the files should be displayed without their extensions
  - The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay)
  - One file name per line
  - The listing should end with a new line
  - You are not allowed to use basename, grep, egrep, fgrep or rgrep

---------------------------------

### [25. Acrostic](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/25-acrostic)

An acrostic is a poem (or other form of writing) in which the first letter (or syllable, or word) of each line (or paragraph, or other recurring feature in the text) spells out a word, message or the alphabet. The word comes from the French acrostiche from post-classical Latin acrostichis). As a form of constrained writing, an acrostic can be used as a mnemonic device to aid memory retrieval.

Create a script that decodes acrostics that use the first letter of each line.

  - The ‘decoded’ message has to end with a new line
  - You are not allowed to use grep, egrep, fgrep or rgrep

------------------------------

### [26. The Biggest Fan](https://github.com/MathieuMorel62/holbertonschool-shell/blob/master/io_redirections_and_filters/26-the_biggest_fan)

Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.

  - Order by number of requests, most active host or IP at the top
  - You are not allowed to use grep, egrep, fgrep or rgrep

--------------------------------
