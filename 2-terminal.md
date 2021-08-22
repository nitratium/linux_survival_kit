*** CHECK cal --before or --Before ***

# So the famous Terminal...

*** Firstly, I need to inform you about something. You know the terminal on Linux right? Well, it's not a terminal.

* We have 3 important terms to learn before typing commands. Terminal, commands and shell.
  * **Terminal** is the window that we type our commands and submit them to shell simply clicking to enter.
  * **Commands** are the stuff we type on our terminal.
  * **Shell** is a program that interprets our commands into a meaning for our computer to be able to execute.

* Let's open the terminal. You can open your terminal with graphical interface basically clicking on its icon on your favorites menu. When you install Ubuntu, terminal icon comes as stock on your favorites menu or taskbar with Windows slang. Also you can use the shortcut **CTRL + ALT + T** to open your terminal.

* I am hoping that you managed to open your terminal. :) 

* Okay, welcome to your terminal. This console allows you to use your computer fully functionally with only typing commands. If you know how to use it, of course.

* Lets talk about command structure for a beginning.

# About command structure

* Each command follows the same structure: 

```
$ commandName -options arguments
```

* Lets take our shutdown command as an example. Do not use the command below without further reading. Because, it basically restarts your computer when you run the command. :)
```
$ shutdown -r now
```
* **Command names** are the names of the commands that we will use. "shutdown" is the name of the command for our example.

#
* We can spesify **options** for a command to customise its behaviour. Some options may have long-form and short-form options. For short-form options we use "-" and for long form options we use "--". Lets assume we have an option a and its long form as alpha. So;
```
Short-form option: -a 
Long-form option: --alpha
```
this two options are equivalent.

* As you can guess, "-r" is an option for our command. This option tells our command to restart the computer after the shutdown. If we wouldn't type -r it would just shut the computer down.

#
* **Arguments** are our inputs. Some commands take only one input while some takes more than one. Some commands take no inputs at all. Shutdown command takes a timing input for the shutdown. We have given "now" input for shutting down "right now".

* Some options may also take arguments. For example:
```
$ cal -B 2 11 2021 
```
or
```
$ cal --before 2 11 2021
```
* This command will return 2 months before of 11/2021 which is 09/2021.

#
* There is something called manual pages on Linux terminal. Most of the commands have detailed information about themselves on these pages. So you don't need to memorise everything. You can navigate through these manual pages only in the terminal, even without an internet connection. I will create a manual page spesific document to show how to use manual pages.

* See you on the next document!