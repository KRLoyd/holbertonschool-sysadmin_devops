# 0x01. Shell, permissions

## Purpose
To be ale to explain:
* Permissions
	* What do the commands `chmod`, `sudo`, `su`, `chown`, and `chgrp` do
	* Linux file permissions
	* How to represent each of the three sets of permissions (owner, group, and other) as a single digit
	* How to change permissions, owner, and group of a file
	* Why can't a normal user `chown` a file
	* How to run a command with root privileges
	* How to change user ID or become superuser
* Other man pages
	* How to create a user
	* How to create a group
	* How to print real and effective user and group IDs
	* How to print the groups a user is in
	* How to print the effective userid

## Tasks
### 0. My name is Betty
Script to change your user ID to `betty`
* File: `0-iam_betty`

### 1. Who am I
Script to print the effective userid of the current user
* File: `1-who_am_i`

### 2. Empty!
Script to create an empty file named `hello`
* File: `4-empty`

### 3. Groups
Script to print all the groups the current user is a part of
* File: `2-groups`

### 4. New owner
Script to change the owner of file `hello` to user `betty`
* File: `3-new_owner`

### 5. Execute
Script to add execute permission to the owner of file `hello`
* Note: `hello` should be in the working directory
* File: `5-execute`

### 6. Mulitple permissions
Script to add execute permission to the owner and group owner, and read permission to other users, to file `hello`
* Note: `hello` should be in the working directory
* File: `6-multiple_permissions`

### 7. Everybody!
Script to add execution permission to owner, gourp, and other users to file `hello`
* Note: `hello` should be in the working directory
* File: `7-everybody`

### 8. James Bond
Script to set the permission for `hello` as follows:
	* Owner: no permissions at all
	* Group: no permissions at all
	* Other users: all permissions
* File: `8-James_Bond`

### 9. John Doe
Script to set the mode of `hello` to `-rwr-x-wx`
* File: `9-John_Doe`

### 10. Look in the mirror
Script to set the mode of file `hello` to the hame as `olleh`'s mode
* Note: both files should be in the working direcotry
* File: 10-mirror_permissions

### 11. Directories
Script to ad execute permission to all subdirectories of the current direcotry for the owner, goupr owner, and other users. 
* Note: Regular files should not be changed
* File: `11-directories_permissions`

### 12. More directories
Script to create a directory with permissions 751 in the working directory
* Directory name: `dir_holberton`
* File: `12-directory_permissions`

### 13. Change group
Script to change the group owner of file `hello` to group `holberton`
* Note: `hello` should be in the working directory
* File: `13-change_group`

### 14. Owner and group
Script to change the owner and group owner for all files and directories in the working directory
* New Owner: `betty`
* New Group Owner: `holberton`
* File: `14-change_owner_and_group`

### 15. Symbolic links
Script to change the owner and group owner of file `_hello`
* New Owner: `betty`
* New Group Owner: `holberton`
* Notes:
	* file `_hello` is in the working directory and is a symbolic link
* File: `15-symbolic_link_permissions`

### 16. If only
Script to change the owner of file `hello` only if it's owned by user `guillaume`
* Note: file `hello` will be in the working directory
* New Owner: `betty`
* File: `16-if_only`

### 17. Star Wars
Script to play Star Wars episode IV in the terminal
* File: `100-Star_Wars`

### 18. RTFM
Man page for holberton.
* File: `101-man_holberton`
