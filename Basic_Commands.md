
# echo Command
* If you have programming experience this thing basically does what a **print()** does. If you don't have any programming experience it is still so easy. Give it an input and it will return what you gave it as argument.

```
$ echo Hello World!
Hello World!
```

* You might think "Why do I need something like this? It just mirrors me.". Well, yes for now it is useless but we can redirect outputs to other commands or to other files. With this power it gains meaning. We will discuss redirection in detail later, don't worry about it now.

# date and cal Command
  * As you can imagine, date returns the current date and time. 
  ```
  $ date
  Tue Jun 27 14:51:22 IST 2021
  ```

  * 'cal' returns an interesting output that I'm pretty sure you will like.
  ```
  $ cal -A -B

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