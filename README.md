# minishell
A simple shell, my own little bash, coded in C

## How to run it
In the project directory type `make` and `./minishell`, now you're in!

## Features
* Show a prompt and wait for a new command
* Search and launch the right executable (based on PATH variable or by using relative or absolute path) like in bash
* Re-implement the builtins:
	* `echo` with option '-n'
	* `cd`
	* `pwd` without any option
	* `export`
	* `unset`
	* `env`
	* `exit`
* `;` separete commands like in bash
* `'` and `"` work like in bash
* Redirection `< > << >>` work like in bash
* Pipes `|` work like in bash
* Environment variables (`$folloew by charcaters`), including `$?` work like in bash
* ctrl-C ctrl-D ctrl-\ work like in bash
* Command history works like in bash
* `&&` and `||` for priorities
* wildcards `*`

Only autocompletion is missing, it would have been a hell to implement it without `readline`

## TOFIX
A late bug occured when adding priorities with `&&`and `||`, all spaces are reduced to one, also the one inside `"` or `'`, so `"__a__b__c"` will traduce in `"_a_b_c"` where `_` equals to space
*** 
  
This project was developed by me and @raccoman
