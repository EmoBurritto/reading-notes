## Bash Command Line Tutorials 

- linux command line is bash 

(reference: https://ryanstutorials.net/linuxtutorial/)

# The Command Line - What is it, how does it work and how do I get to one.

command line (also known as a terminal) running Bash

ls -l /home/ryan
- ls is list is the command 
-l /home/ryan is the command line argument
-l is the option
options usually started with dash  

most commands produce output, others no response like git commit -m""

when prompt is present again, command finished and all output is displayed

shell = This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you

bash which stands for Bourne again shell, most common shell 

up and down arrow keys on empty prompt to view input history

(reference: https://ryanstutorials.net/linuxtutorial/commandline.php)

# Basic Navigation - An introduction to the Linux directory system and how to get around it.

pwd stands for Print Working Directory

ls is short list to know where we are, also short list of files 

ls [options] [location] is ls -l /etc

-l long list 

d is directory 

/etc is to list contents not including current directory 

A path is a means to get to a particular file or directory on the system

file system under linux is a hierarchical structure

at the top is root directory; single /

two type of paths 

absolute specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / ); ls /home/ryan/Documents

relative  specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash; ls Documents 

~ is a tilde, short cut to avoid / in root directory 

. current directory 

.. parent directory

cd change directory 

tab completion is a blessing and a curse 

(reference: https://ryanstutorials.net/linuxtutorial/navigation.php)

# More About Files - Find out some interesting characteristics of files and directories in a Linux environment.

everything is a file in linux 

file extension is normally 2-4 set characters 

- file.exe - an executable file, or program.

- file.txt - a plain text file.

- file.png, file.gif, file.jpg - an image.

Linux the system actually ignores the extension and looks inside the file to determine what type of file it is

file [path] helps determine what the file type is without relying on the extension

linux is case sensitive 

bets not to use spaces for file names, use camel casing 

spaces used for separating items 

can used single or double quotes, best to just use double and everything inside quote is single item like a git commit -m""

\ or escape character negates teh next character in sequence 

- Holiday\ Photos is Holiday Photos 

ls -a for hidden files 

(reference: https://ryanstutorials.net/linuxtutorial/aboutfiles.php)

# Manual Pages - Learn how to make the most of the Linux commands you are learning.

manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept

man <command to look up>

-a = --all is do not ignore entries starting with

-A = --almost-all is    do not list implied . and ..

To exit the man pages press 'q' for quit

man -k <search term> is manual keyword search 

/<term> is Within a manual page, perform a search for 'term'

use manual pages when lost or use google to see what command is completely lost but then use manual for practice 

(reference: https://ryanstutorials.net/linuxtutorial/manual.php)

# File Manipulation - How to make, remove, rename, copy and move files and directories.

mkdir [options] <Directory> to make a new directory 

command line options 

-p which tells mkdir to make parent directories as needed 

-v which makes mkdir tell us what it is doing

rmdir [options] <Directory> to remove a directory 

IMPORTANT: a directory must be empty before it may be removed

touch [options] <filename> to make empty file 

did not know the touch file technique to appear like work is done  

cp [options] <source> <destination> to copy file only

If you provide a directory as the destination then it will copy the file into that directory and the copy will have the same name as the source

 -r option is to copy directories

 mv [options] <source> <destination> to move file or directory 

 rm [options] <file> to remove file EMPTY directory

 rm -r to remove non EMPTY directory 

(reference: https://ryanstutorials.net/linuxtutorial/filemanipulation.php)

# Cheat Sheet - A quick reference for the main points covered in this tutorial.

Here are some very complicated or just fun commands I found that I can see useful down the line:

basename -s .jpg -a *.jpg | xargs -n1 -i cp {}.jpg {}_original.jpg
Make a copy of every jpg image file in the current directory and rename adding _original.

Hidden files and directories
A name beginning with a . (dot) is considered hidden.

df -h
Display how much disk space is used and also free.

shutdown -h now
Shutdown the system. (Replace -h with -r for reboot.)


(reference: https://ryanstutorials.net/linuxtutorial/cheatsheet.php)