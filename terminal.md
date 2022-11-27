# Terminal Practice

## The Command Line - What is it, how does it work and how do I get to one

- A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.  If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.
If you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .

## Basic Navigation - An introduction to the Linux directory system and how to get around it

- Commands to find out where we are in the terminal
pwd
Print Working Directory - ie. Where are we currently.
ls
List the contents of a directory.
cd
Change Directories - ie. move to another directory.

Diffrent Paths

Relative path
A file or directory location relative to where we currently are in the file system.
Absolute path
A file or directory location in relation to the root of the file system.

## More About Files - Find out some interesting characteristics of files and directories in a Linux environment

- Ok, the first thing we need to appreciate with linux is that under the hood, everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc. To begin with, this won't affect what we do too much but keep it in mind as it helps with understanding the behaviour of Linux as we manage files and directories.

- To make a file or directory hidden all you need to do is create the file or directory with it's name beginning with a . or rename it to be as such. Likewise you may rename a hidden file to remove the . and it will become unhidden. The command ls which we have seen in the previous section will not list hidden files and directories by default. We may modify it by including the command line option -a so that it does show hidden files and directories.

- Linux is an extensionless system
- Files can have any extension they like or none at all.
- Linux is case sensitive
- Beware of silly typos.

## Manual Pages - Learn how to make the most of the Linux commands you are learning

- The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. Some of them are a little hard to get your head around but they are fairly consistent in their structure so once you get the hang of it it's not too bad. You invoke the manual pages with the following command:

man <command to look up>

-It is possible to do a keyword search on the Manual pages. This can be helpful if you're not quite sure of what command you may want to use but you know what you want to achieve. To be effective with this approach, you may need a few goes. It is not uncommon to find that a particular word exists in many manual pages.

man -k <search term>

## File Manipulation - How to make, remove, rename, copy and move files and directories

mkdir
Make Directory - ie. Create a directory.
rmdir
Remove Directory - ie. Delete a directory.
touch
Create a blank file.
cp
Copy - ie. Copy a file or directory.
mv
Move - ie. Move a file or directory (can also be used to rename).
rm
Remove - ie. Delete a file.

## Cheat Sheet - A quick reference for the main points covered in this tutorial

[Cheat Sheet Link](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
