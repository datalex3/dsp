# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

* show current working directory path           pwd
* creating a directory                          mkdir
* deleting a directory                          rmdir
* creating a file using `touch` command         touch file_name
* deleting a file                               rm file_name
* renaming a file                               mv old_name new_name
* listing hidden files                          ls -a
* copying a file from one directory to another  cp file_name /new_dir
* change directory                              cd dir_name
* show content of file                          cat file_name

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

`ls`       list files in  a folder
`ls -a`    list all files 
`ls -l`    list file details
`ls -lh`   detailed human readable
`ls -lah`  all files details human readable
`ls -t`    list files in order by time
`ls -Glp`  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:
'ls -c' list files by timestamp
'ls -d' list of directories
'ls -r' list in reverse order
'ls -m' list as comma separated
'ls -1' list each on one line


> > 
---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Allows for building and executing of commands. The output from one command can become the input for another command by utilizing xargs.
Example:
Xargs in conjuction with grep could be utilized to search through files containing a particular string. 
find -name "*.txt" | xargs grep "metis"
 

