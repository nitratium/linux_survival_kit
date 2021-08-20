
# So the famous Terminal...

*** Firstly, I need to inform you about something. You know the terminal on Linux right? Well, it's not a terminal.

* Let's open the terminal. You can open your terminal with graphical interface basically clicking on its icon on your favorites menu. When you install Ubuntu terminal icon comes as stock on your favorites menu or taskbar with Windows slang. Or you can use the shortcut **CTRL + ALT + T** to open your terminal.

* I am hoping that you managed to open your terminal :). 

* Okay, welcome to your terminal. This console allows you to use your computer fully functionally with only typing commands. If you know how to use it, of course.

* Lets try an easy commands for start.

# About command structure

* Each command follows the same structure: 

```
$ commandName -options arguments
```

* Lets take our shutdown command for example.

```
$ shutdown -r now
```

* **Command names** are the names of the commands that we will use. We should have them installed on our computer. We will come to installing and removing commands later.
"shutdown" is the name of the command for our example.

* We can spesify **options** for a command to customise its behaviour. Some options has long-form and short-form options. For short-form options we use only one "-" and for long form options we use "--". Lets assume we have an option a. And its long form is alpha. So:
```
Short-form option: -a 
Long-form option: --alpha
```
this two options are equivalent.
* As you can guess, "-r" is an option for our command. This option tells our command to restart the computer. If we wouldn't type -r it would just shut the computer down.

* **Arguments or inputs** are the third part of our commands.


* Some options may also take arguments. For example:
```
$ cal -B 2 11 2021 
```
or
```
$ cal --before 2 11 2021
```
* This command will return 2 months before of 11/2021 which is 09/2021.


*** CHECK cal --before or --Before ***