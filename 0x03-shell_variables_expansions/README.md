# 0x03. Shell, init files, variables and expansions

## Purpose
To be able to explain the following:
* Shell initialization files
	* What are the `/etc/profile` file and `/etc/profile.d` directory
	* What is the file `~/.bashrc`
* Variables
	* What is the difference between a local and a global variable
	* What is a reserved variable
	* HOw to create, update and delete shell variables
	* What are the roles of the reserves variable HOME, PATH, and PSI
	* What are special parameters
	* What is the special parameter `$?`
* Expansions
	* What is expansion and how to use them
	* What is the difference between single and double quotes and how to use them properly
	* How to do command substitution with `$()` and backticks
* Expansions & Shell Arithmetic
	* How to perform arithmetic operations with the shell
* The alias Command
	* How to create an alias
	* How to list aliases
	* How to temporarily disable an alias
* Other help pages
	* How to execute commands from a file in the current shell
* And
	* What happens when you type `$ ls -l *.txt`


### Project Notes
* Scripts should be 2 lines long (this can be tested with `$ wc -l file`)

## Tasks

#### 0. <o>
Script that creates alias `ls` with a value of `rm *`.
* File: `0-alias`

#### 1. Hello you
Script that prints `hello user`, where `user` is the current Linux user.
* File: `1-hello_you`

#### 2. The path to success is to take massive, determined action
Script that adds `/action` to the `PATH`.
* File: `2-path`

#### 3. If the path be beautiful, let us not ask where it leads
Script that counts the number of directories in the `PATH`.
* File: `3-paths`

#### 4. Global Variables
Script that lists environment variables.
* File: `4-global_variables`

#### 5. Local variables
Script that lists all local variables, environment variables, and functions.
* File: `5-local_variables`

#### 6. Local variable
Script that creates new local variable named `BETTY` with value of `Holberton`.
* File: `6-create_local_variable`

#### 7. Global Variable
Script that creates a new global variable named `HOLBERTON` with the value of `Betty`.
* File: `7-create_global_variable`

#### 8. Every addition to true knowledge is an addition to human power
Script that prints the result of 128 added to the value stored in the environment variable `TRUEKNOWLEDGE`.
* File: `8-ture_knowledge`

#### 9. Divide and rule
Script that prints the result of `POWER` divided by `DIVIDE`; they are both environment variables.
* File: `9-divide_and_rule`

#### 10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath
Script that displays the result of `BREATH` to the power of `LOVE`; both are environmental variables.
* File: `10-love_exponent_breath`

#### 11. There are 10 types of people in the world -- Those who understand binary, and those who don't
Script that converts a number from base 2 to base 10. 
* Note: Number in base 2 is stored in environment variable `BINARY`
* File: `11-binary_to_decimal`

#### 12. Combination
Script that prints all possible combinations of two letters, excluding `oo`.
* Notes:
	* Letters are lowercase, from `a` to `z`
	* Displayed as one combination per line and in alpha order
* File: `12-combinations`

#### 13. Floats
Script that prints a number with two decimal places. 
* Note: the number to be printed is stored in environment variable `NUM`
* File: `13-print_float`

#### 14. Decimal to Hexadecimal
Script that converts a number from base 10 to base 16. 
* Note: the base 10 number to convert is stored in environment variable `DECIMAL`

#### 15. What happens when you type `ls *.c`
Blog post describing what happens when you type `ls *.c` and hit Enter in your shell. 
* Blog: https://medium.com/@loydkristen/detective-decoders-episode-1-6b1d152c1107#.l9kyh1sa6

#### 16. What is the difference between a hard link and a symbolic link?
Blog post explaining what hard and symbolic links are on Linux, how to create them, and the difference between the two. 
* Blog: https://medium.com/@loydkristen/hard-links-symbolic-links-fd2bcd16c46e#.add3g5olp

#### 17. Everyone is a proponent of strong encryption
Script that encodes and decodes text using the rot13 encryption.
* File: `100-rot13`

#### 18. The eggs of the brood need to be an odd number
Script that prints every other line from the input, starting with the first line. 
* File: `101-odd`

#### 19. I'm an instant star. Just add water and stir. 
Script that adds two numbers in the environment variables `WATER` and `STIR` and prints the result. 
* Notes:
	* `WATER` is in base `water`
	* `Stir` is in base `stir`
	* Result is in base `behlnort`
* File: `102-water_and_stir`
