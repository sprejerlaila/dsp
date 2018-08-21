# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path: pwd
* creating a directory: mkdir
* deleting a directory: rmdir
* creating a file using `touch` command
* deleting a file: rm
* renaming a file: mv 
* listing hidden files: ls -a
* copying a file from one directory to another: cp

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
- cd: go to a directory
- man -k <search term>: looks in every manual pages for the search term
- touch: create blank file
- ls *.???: show every file with a 3 letter extension. *: zero or more characters. ?: one character
- chmode: change permissions.
- vi: view / edit file. 
- cat: view / concatenate files.
- head / tail: print first/last rows of a file (10 by default).
- sort: sorts a file
- wc: words count of a file
- sed: search and replace. s/search/replace/g

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > ls: lists all files in a directory
> > ls -a: lists all files in a directory (even the hidden files)
> > ls -l: displays the long format listing
> > ls -lh: displays the long format listing with sizes in human readable format
> > ls -lah: displays all filez with the long format listing with sizes in human readable format
> > ls -t: sorts by modification time
> > ls -Glp: do not print group names, and shows directories with /. 

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -d: displays only directories
> > ls -R: displays subdirectories as well
> > ls -m: displays the names as a comma separated list
> > ls -f: interprets each name as a directory, not a file
> > ls -S: sort by file size, largest first

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs converts inputs into arguments to execute a command. 
echo 'folder1 folder2 folder3' | xargs mkdir --> creates three folders, folder1 folder2 and folder3
 

