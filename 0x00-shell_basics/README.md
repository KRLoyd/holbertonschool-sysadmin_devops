# 0x00. Shell, basics

## Purpose
To be able to explain the following:
* What is "The Shell"?
	* What is the shell?
	* What is the difference between a terminal and a shell?
	* What is the shell prompt?
	* How to use the history (basics)
* Navigation
	* What do the commands of built-ins `cd`, `pwd`, and `ls` do?
	* How to navigate the filesystem
	* What is the working directory, how to print or change it
	* What is the root directory?
	* What is the home directory and how to go there
	* What is the difference between the root directory and the home directory of user root?
	* What are the characteristics of hidden files and how to list them
	* What does the command `cd -` do
* Looking around
	* What do the commands `ls`, `less`, and `file` do
	* How do you use options and arguments with commands
	* Understanding the `ls` long format and how to display it
* A Guided Tour
	* What does the `ln` command do?
	* What do you find in the most common/important directories
	* What is a symoblic link
	* What is a hard link
	* What is the difference between a hard link and a symbolic link
* Manipulating files
	* What do the commands `cp`, `mv`, `rm`, and `man` do?
	* What are wildcards and how do they work
	* How to use wildcards
* Working with commands
	* What do `type`, `which`, `help`, and `man` commands do
	* What are the different kinds of commands
	* What is an alias
	* When do you use the command help instead of man
* Reading Man Pages
	* How to read a man page
	* What are man page sections
	* What are the section numbers for User commands, System calls, and Library functions
* Keyboard shortcuts for Bash
	* Common shortcuts for Bash
* LTS
	* What does `LTS` mean
* Other
	* What does RTFM mean
	* What is a Shebang

#### General Notes for these tasks
* All scripts must be executable, use `chmod u+x file_name`


## Tasks
### 0. Where am I?

Script that prints the absolute path name of the current working directory.
* File: `0-current_working_directory`

### 1. What's in there?

Script to display the contents list of your current directory. 
* File: `1-listit`

### 2. There is no place like home

Script to change the working directory to the user's home directory. 
* File: `2-bring_me_home`

### 3. The long format

Script to display current directory contents in a long format. 
* File: `3-listfiles`

### 4. Hidden files

Script to display current directory contents, including hidden files, using the long format. 
* File: `4-listmorefiles`
* Note: hidden files begin with `.`

### 5. I love numbers

Script to display the current directory contents with the following:
* Long format
* user and group IDs displayed numerically
* show hidden files

* File: `5-listfilesdigitonly`

### 6. Welcome holberton

Script to create a directory in the `/tmp/` directory
* Directory to create: `holberton`
* File: `6-firstdirectory`

### 7. Betty in Holberton

Script to move `betty` from `/tmp/` to `/tmp/holberton`
* File: `7-movethatfile`

### 8. Bye bye Betty

Script to delete `betty` from `/tmp/holberton`
* File: `8-firstdelete`

### 9. Bye bye Holberton

Script to delete directory `holberton` from `/tmp`
* File: 9-firstdirdeletion

### 10. Back to the future

Script to change the working directory to the previous one. 
* File: `10-back`

### 11. Lists

Srcipt to list all files in the current directory, parent of working directory, and `/boot` directory in long format.
* File: `11-lists`

### 12. File type

Script to print the type of the file `iamafile`
* `iamafile` will be in `/tmp` directory
* File: `12-file_type`

### 13. We are symbols, and inhabit symbols

Create a symbolic link to `/bin/ls` in your current working directory
* Symbolic link name: `__ls__`
* File: `13-symbolic_link`

### 14. Copy HTML files

Script to copy all HTML files from current working directory to the parent directory.
* Only copy files that didn't exist in the parent direcotry or were newer versions of what is in the parent directory
* File: `14-copy_html`

### 15. Let's move

Script to move all files beginning with an uppercase letter to `/tmp/u` directory
* File: `15-lets_move`

### 16. Clean Emacs

Script to delete all files in corrent working directory that end with `~`
* File: `16-clean_emacs`

### 17. Tree

Script to create directories in the current directory
* Note: only allowed 2 spaces in script
* Directories to create: 
	* `welcome/`
	* `welcome/to`
	* `welcome/to/holberton`
* File: `17-tree`

### 18. Life is a series of commas, not periods

Command to list all files and directories of the current direcotries
* Notes:
	* seperate by commas (`,`)
	* directories should end with a slash (`/`)
	* list hidden files and directories
	* `.` and `..` files should be first, with all others in alphabetical order
	* digits should come first
	* listing ends in newline
* File: `18-commas`

### 19. File type: Holberton

Create a magic file that can be used with command `file` to detect `Holberton` data files. 
* Note: `Holberton` type files contain the string `HOLBERTON` at offset 0
* Magic file to create: `holberton.mgc`
