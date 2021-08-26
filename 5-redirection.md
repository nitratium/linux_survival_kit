# File Descriptors
  * File descriptors (FDs) are like pointers to sources data can be read or places data can be written. There are three file descriptors:
    * Standard Input (stdin): FD 0
    * Standard Output (stdout): FD 1
    * Standard Error (stderr): FD 2

  * Standard Input is your keyboard basically. Standard Output is where the program returns its output and Standard Error is where the program sends its error messages. Mostly Standard Output and Standard Error directed to your terminal and Standard Input is set to your keyboard by default. But we can redirect them. Does it sounds meaningless? If yes, then you are going to understand what it is with following examples don't worry. Just keep going. These are just definitions, mostly they don't make sense, aren't they? :)

  # Redirection
  * As we discussed earlier, we are able to redirect our file descriptors to different sources and different places.
    * For redirecting Standard Input Stream, we should use the operator **"0<"** or **"<"**. 
    ```
    $ command_name –options arguments 0< source_destination
    ```
    or
    ```
    $ command_name –options arguments < source_destination
    ```

    * For redirecting Standard Output Stream, we should use the operator **"1>"** or **">"**.
    ```
    $ command_name –options arguments 1> output_destination
    ```
    or 
    ```
    $ command_name –options arguments > output_destination
    ```

    * For redirecting Standard Error Stream, we should use the operator **"2>"**.
    ```
    $ command_name –options arguments 2> error_destination
    ```
      * There is no short from for this. :(
    
  #
  * Let's redirect stuff into text files and read inputs from text files. You don't need to create any text file on your desktop. If there is none, commands will create one for you. Also you can observe the creation on your graphical interface after you run the commands. 
  * Don't worry about file paths for now. We will discuss about them in detail on later documents. If commands doesnt work because of the path, use **"cd"** command for once and they should work. If you are curious, we are using cd command for navigating through directories. It is short for "change direction". If you don't give any input to cd, it will teleport you into your home directory.

  * Standard Output Example:
    ```
    $ date 1> Desktop/date.txt
    ```
    * Now go inside that text file with your graphical interface or just type "cat Desktop/date.txt" on the terminal and check what file contains inside. Isn't that exciting?
    * Reminder: we can also use the ">" operator to direct our input. 

  * Standard Input Example:
    * Let's try to read that file with echo command while redirecting our input from keyboard to text file.
    ```
    $ xargs echo 0< Desktop/date.txt
    ```
    * This should return the content of date.txt file.
    * Reminder: We can also use the "<" operator to direct our input. 
    * I will explain xargs on next document. Ignore that for now.

  * Standard Error Example:
    * For redirecting an error message we should get an error message first, right? So, let's do something illegal for Linux Terminal and redirect error output to text file.
    ```
    $ cal imDoingSomethingWrong 2> Desktop/date.txt
    ```
    * Do you remember what cal command were getting as argument? Yes, the date as numbers. So, you should see the error message in date.txt.
    * Did you notice that redirecting output to same text file has overwritten everything in the text file? If you don't want it to overwrite the text file, using "1>>" and "2>>" is going to solve your problem.

  [For more information, check the Official GNU manual.](https://www.gnu.org/software/bash/manual/html_node/Redirections.html)
 #
 * See you on the next document!
