[[Template:Milestone 2]]
The Console is a panel normally hidden from view. Its usage is twofold:

* It displays informational, warning and error messages that occur during gameplay, alerting players of things like low diskspace, broken levels, ...
* It helps debug the engine and test levels by allowing direct execution of Squirrel script commands (see [[Scripting reference]])

The Console pops into view for a short time whenever new messages are printed. To review old messages and enter commands, the console needs to be activated.

To do so, you will have to run supertux using the <tt>--console</tt> option. The key assigned to opening the console can be changed in the keyboard setup as soon it is activated. (Default of ^) Use <tt>--noconsole</tt> to disable it again.

To disable or enable the console if you don't want to pass command line parameters, you will have to edit the edit the SuperTux configuration file. Depending on your operating system, this varies:
{| border="1"
! align="left" | Operating System !! align="left" | Config file location
|-
| align="left" | Linux            || align="left" | ~/.supertux2/config
|-
| align="left" | Windows          || align="left" | %USERPROFILE%\.supertux2\config
|-
| align="left" | Mac OS X         || align="left" | ~/Library/Application Support/SuperTux/config.txt
|-
| align="left" | Mac OS X Leopard || align="left" | ~/.supertux2/config
|-
| align="left" | Mac OS X Leopard (Wine) || align="left" | ~/Library/Application Support/Wine/Prefixes/drive_c/Program FIles/(Name of your Supertux)/.supertux2/config
|}

You may have to enable viewing hidden files or folders.
Anyway, open the file up with a text editor, and
  (console #t)
will enable the console, and 
  (console #f)
will disable the console. Find one to change it to the other.

== Commands ==

Following is a list of predefined scripts to run in the console:
{|
|'''flip()'''||Flips the current level vertically. Make sure you have something to stand on!
|-
|'''edit()'''||Puts the level into a state suitable for testing out edits. Tux can't exit the level; if he dies or reaches the end he goes into ghost mode.
|-
|'''play()'''||Goes out of edit mode and restarts the level.
|-
|'''kill()'''||Kills Tux
|-
|'''grow()'''||Grows Tux into big Tux
|-
|'''shrink()'''||Shrinks Tux into little Tux
|-
|'''fire()'''||Gives Tux the fire powerup
|-
|'''ice()'''||Gives Tux the ice powerup
|'''air()'''||Gives Tux the air powerup
|-
|'''earth()'''||Gives Tux the earth powerup
|-
|'''lifeup()'''||Gives Tux 100 more coins
|-
|'''finish()'''||Finish the current level
|-
|'''worldmapfinish()'''||Finish all the levels on the worldmap
|-
|'''functions(x)'''||Gives a list of the functions available in an object or table. If no argument is given, this prints out the functions in the root table.
|}

There are many more, see [[ScriptingGlobals]] for the full list of utility functions and [[Scripting reference]] for all the interesting things you can do.

== Console Features ==
The console currently supports autocomplete, through use of the tab key, line editing with left/right/home/end/delete keys, and viewing past messages using the up, down, page up, and page down keys. To run a command, simply press the enter or return key.

[[Category:Game Engine]]