# 0x02. Shell, I/O Redirections and filters

## Purpose
To be able to explain the following:
* Shell, I/O Redirection
	* What do the commands `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr` do
	* How to redirect standard output to a file
	* How to get standard input from a file instead of the keyboard
	* How to send the output from one program to the input of another program
	* How to combine commands and filters with redirections
* Special Characters
	* What are special characters
	* Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde, and how and when to use them
* Other man pages
	* How to display a line of text
	* How to concatenate files and print on the standard output
	* How to reverse a string
	* How to remove sections from each line of files
	* What is the `/etc/passwd` file and what is its format
	* What is the `/etc/shadow` file and what is its format

### Project Requirements
* Scripts should be 2 lines long (this can be checked with `$ wc -l file` output should be 2)
* Files must be executable

## Tasks

#### 0. Hello World
Script that prints "Hello, World" followed by a new line to the standard output.
* File: `0-hello_world`

#### 1. Confused smiley
Script that displays a confused smiley: `"(Ôo)'`
* File: `1-confused_smiley`

#### 2. Let's display a file
Script to display the content of file `/etc/passwd`
* File: `2-hellofile`

#### 3. What about 2?
Script that displays the content of `/etc/passwd` and `/etc/hosts`
* File: `3-twofiles`

#### 4. Last lines of a file
Script that displays the last 10 lines of `/etc/passwd`
* File: `4-lastlines`

#### 5. I'd prefer the first ones actually
Script that displays the first 10 lines of `/etc/passwd`
* File: `5-firstlines`

#### 6. Line #2
Script that displays the third line of file `iacta`
* Notes:
	* File `iacta` should be in the working directory
	* Cannot use `sed`
* File: `6-third_line`

#### 7. Save current state of directory
Script that writes into file `ls_cwd_content` the result of command `ls -la`
* Note: if file `ls_cwd_contect` does not exist, it will be created. If it does exist, it will be overwritten
* File: `8-cwd_state`

#### 8. It is a good file that cuts iron without making a noise
Script that creates a file with a specified name with specified contents.
* File to be created: `\*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:)`
* Contents to be in file: `Holberton School` ending with a new line
* File: `7-file`

#### 9. Duplicate last line
Script that duplicates the last line of file `iacta`
* Note: `iacta` should be in the working directory
* File: `9-duplicate_last_line`

#### 10. No more javascript
Script that deletes all the regular files with a `.js` extension in the current directory and all sub-directories
* File: `10-no_more_js`

#### 11. Don't just count your directories, make your directories count
Script that counts the number of directories and sub-directories in the current directory.
* Notes:
	* Current and parent directories are not taken into account
	* Hidden directories are counted
* File: `11-directories`

#### 12. What's new
Script that displays the 10 newest files in the current directory. 
* Notes:
	* Displays one file per line
	* Sorted from newest to oldest
* File: `12-newest_files`

#### 13. Being unique is better than being perfect
Script that takes a list of words as input and prints only words that appear once. 
* Notes: 
	* Input format: One line per word
	* Output format: One line per word
	* Words are sorted
* File: `13-unique`

#### 14. It must be in that file
Script that displays lines containing the pattern "root" from file `/etc/passwd`
* File: `14-findthatword`

#### 15. Count that word
Script to display the number of lines that contain the pattern "bin" in file `/etc/passwd`
* File: `15-countthatword`

#### 16. What's next?
Script that displays lines containing the pattern "root" and 3 lines after them in file `/etc/passwd`
* File: `16-whatsnext`

#### 17. I hate bins
Script that displays all lines in file `/etc/passwd` that don't contain pattern "bin"
* File: `17-hidethisword`

#### 18. Letters only please
Script that displays all lines of the file `etc/ssh/sshd_config` that start with a letter (lower- or uppercase)
* File: `18-letteronly`

#### 19. A to Z
Script to replace all characters `A` and `c` from input to `Z` and `e`, respectively. 
* To run: `$ echo 'string_to_evaluate' | ./19-AZ`
* File: `19-AZ`

#### 20. Without C, you would live in hiago
Script to remove all letters `c` and `C` from input. 
* To run: `$ echo word_to_evaluate | ./20-hiago`
* File: `20-hiago`

#### 21. esreveR
Script that reverses its input.
* To run: `$ echo "string_to_evaluate" | ./21-reverse`
* File: `21-reverse`

#### 22. DJ Cut Killer
Script that displays all users and their home directories, based on file `/etc/passwd`
* Note: Sorted by users
* File: `22-users_and_homes`

#### 23. Empty casks make the most noise
Command that finds all empty files and directories in the current directory and all sub-directories.
* Notes:
	* Displayed as one file name per line and ends in new line
	* Names of files and directories are displayed without the entire path
	* Hidden files are listed
* File: `100-empty_casks`

#### 24. A gif is worth ten thousand words
Script that lists all the files with `.gif` extension in current directory and all its sub-directories.
* Notes:
	* Hidden files are listed
	* Only regular files are listed
	* Names of files are displayed without extensions
	* Files are sorted by byte values
	* Displays one file per line
* File: `101-gifs`

#### 25. Acrostic
Script that decodes acrostics that use the first letter of each line. 
* File: `102-acrostic`

#### 26. The biggest fan
Script that parses web servers logs in TSV format as input and displays the 11 hosts of IP addresses which did the most requests.
* Note: Output is ordered by number of requests.
* File: `103-the_biggest_fan`
