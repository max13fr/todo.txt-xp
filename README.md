xp
==

XP - A todo.txt module designed to print a readable guide of your accomplishments. 

 Currently XP prints the tasks completed on each day starting (x) number of days ago. 
 
Forked from gr0undzer0/xp to add several improvements :
* search in `$TODO_FILE` and `$DONE_FILE` (originaly, only in `$DONE_FILE`)
* improve display :
 * remove file path & complete time from result lines
 * move creation date to the end
 * add color for context, project and creation date
* clean code (matching regex, indendation, duplication, ...)

Installation: 
-------------

1) Confirm the location of your todo actions directroy. The `TODO_ACTIONS_DIR` variable can be found in `todo.cfg`
2) Copy the XP add-on in the todo actions directory. 

```
~/.todo.actions.d
wget https://raw.githubusercontent.com/max13fr/todo.txt-xp/stable/xp
chmod +x xp
```

Usage: 
------

      todo.sh xp [-oh] days 
              days: Number of days ago.
        
        Options:
              o : Omit days on which no tasks were commited.
              h : Print this help message.

Notes: 
-----

If You experience bad interpreter errors:
Please check for the location of bash. I test on fedora where everything has been moved to `/usr/bin`.

Contact:
--------

   * **xp**: christopher.donald.jones@gmail.com or https://github.com/gr0undzer0/xp
   * **todo.txt**: http://blog.todotxt.com/ or https://github.com/ginatrapani/todo.txt-cli 
