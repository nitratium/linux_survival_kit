*** EXPLAIN HOW TO WORK ON .bash_aliases FILE

# Aliases
 * Aliases allows you to save your commands or pipelines you created. Basically, you write them to a file and give them a memorable nickname with an easy syntax. Let me show you how.
 #

 * First we need to be sure you have a file called .bash_aliases on your home directory. For checking that:
 ```
 $ cd
 $ ls -a
 ```
 * In the printed list, if you see a file called ".bash_aliases", you are good to go. If not:
 ```
 $ touch .bash_aliases
 ```
 * Now check again, you should have the file.
 #
 
 * Let's define some aliases. Aliases should be structured as:
 ```
 $ alias nickname="your custom command"
 ```
 * Note that there are no spaces between markers.
 * Let's take an example:
  ```
  $ alias date_cal_printer="date | tee time.txt | xargs echo >> time.txt"
  ```
  * Now this command should print the date and time in time.txt without overwriting each other.