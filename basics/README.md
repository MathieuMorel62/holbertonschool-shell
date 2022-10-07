SHELL, BASICS


RESOURCES

   Read or watch:

      => What Is "The Shell" ?  -----> https://intranet.hbtn.io/rltoken/aygkrwOyI_yLtXHF1Yj0QQ

      => Navigation  -----> https://intranet.hbtn.io/rltoken/fMDkg3TKjANJSPTROMQSpA

      => Looking Around  -----> https://intranet.hbtn.io/rltoken/isPTWCOgTjeLaonZg8Rl5g

      => A Guided Tour  -----> https://intranet.hbtn.io/rltoken/GznRkhU3QTWAWwDeZ-k9Pw

      => Manipulating Files  -----> https://intranet.hbtn.io/rltoken/GA2UvOhDOjwa-NtbazvlCQ

      => Working With Commands  -----> https://intranet.hbtn.io/rltoken/ylGnKaanTSp3jIpXme9krg

      => Reading Man Pages  -----> https://intranet.hbtn.io/rltoken/52aXMywgSkXV07rFrX8eWw

      => Keyboard Shortcuts For Bash  -----> https://intranet.hbtn.io/rltoken/XXe2AD3TVWvNFwSP5_-YWQ

      => LTS  -----> https://wiki.ubuntu.com/LTS

      => Shebang  -----> https://intranet.hbtn.io/rltoken/_pJ5Fl2TaZVzW3jJy_mwKA



TASKS

0. WHERE AM I ?

   Write a script that prints the absolute path name of the current working directory.


1. WHAT'S IN THERE ?

   Display the contents list of your current directory.


2. THERE IS NO PLACE LIKE HOME

   Write a script that changes the working directory to the user’s home directory.

      => You are not allowed to use any shell variables


3. THE LONG FORMAT

   Display current directory contents in a long format


4. HIDDEN FILES

   Display current directory contents, including hidden files (starting with .). Use the long format.


5. I LOVE NUMBERS

   Display current directory contents.

      => Long format

      => with user and group IDs displayed numerically

      => And hidden files (starting with .)


6. WELCOME

   Create a script that creates a directory named my_first_directory in the /tmp/ directory.


7. BETTY IN MY FIRST DIRECTORY

   Move the file betty from /tmp/ to /tmp/my_first_directory.


8. BYE BYE BETTY

   Delete the file betty.

      => he file betty is in /tmp/my_first_directory


9. BYE BYE MY FIRST DIRECTORY

   Delete the directory my_first_directory that is in the /tmp directory.


10. BACK TO THE FUTURE

    Write a script that changes the working directory to the previous one.


11. LISTS

    Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.


12. FILE TYPE

    Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.


13. WE ARE SYMBOLS, AND INHABIT SYMBOLS

    Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory.


14. COPY HTML FILES

    Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

    You can consider that all HTML files have the extension .html


15. LET'S MOVE

    Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u.

    You can assume that the directory /tmp/u will exist when we will run your script


16. CLEAN EMACS

    Create a script that deletes all files in the current working directory that end with the character ~.


17. TREE

    Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.

    You are only allowed to use two spaces (and lines) in your script, not more.
