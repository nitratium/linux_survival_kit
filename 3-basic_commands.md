*** CAL COMMAND MISSING

# echo Command
* If you have programming experience this thing basically does what a **print()** does. If you don't have any programming experience it is still so easy. Give it an input and it will return what you gave it as argument.

```
$ echo Hello World!
Hello World!
```

* You might think "Why do I need something like this? It just mirrors me.". Well, yes for now it is useless but we can redirect outputs to other commands or to other files. With this power it gains meaning. We will discuss redirection in detail later, don't worry about it now.

# date and cal Command
  ### date
  * As you can guess, date returns the current date and time. 
  ```
  $ date
  Tue Jun 27 14:51:16 +03 2021
  ```
  ### cal
  * 'cal' returns an interesting output that I'm pretty sure you are going to like.
  ```
  $ cal 09 2021
      August 2021       
Su Mo Tu We Th Fr Sa  
 1  2  3  4  5  6  7  
 8  9 10 11 12 13 14  
15 16 17 18 19 20 21  
22 23 24 25 26 27 28  
29 30 31  
  ```
  
  * cal has 2 command line arguments. First one is the day of a month and second one is the month.
```
  $ cal -A1 -B1 09 2021
  
      August 2021          September 2021         October 2021      
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  
 1  2  3  4  5  6  7            1  2  3  4                  1  2  
 8  9 10 11 12 13 14   5  6  7  8  9 10 11   3  4  5  6  7  8  9  
15 16 17 18 19 20 21  12 13 14 15 16 17 18  10 11 12 13 14 15 16  
22 23 24 25 26 27 28  19 20 21 22 23 24 25  17 18 19 20 21 22 23  
29 30 31              26 27 28 29 30        24 25 26 27 28 29 30  
                                            31   
 ```

# history Command
* Returns all the commands that you have entered before.
```
$ history
```
  * -c option will clear your history cache.
  ```
  $ history -c
  ```
  * "!!" will run the previous command. !x will run your xth command.
  ```
  $ echo Hello World!
  Hello World!
  $ !!
  Hello World!
  ```
  and
  ```
  $ !34
  ```
  will run your 34th command on your history list.

  * Also you can navigate through old commands with up and down arrow keys without using history command.

# cat Command
* This command returns the content of any file. Mostly we use this for text files.
  * Lets assume that we have a text file named text.txt with the content "This is a text file.".
  ```
  $ cat text.txt
  This is a text file.
  ```

# whoami Command
* This command prints current user's name. Basically, it tells you who you are.
  ```
  $ whoami
  nitrat
  ```
* nitrat is my username on my Linux. Of course you should see your own nickname. :)
#
* See you on the next document!
