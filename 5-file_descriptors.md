# File Descriptors
  * File descriptors (FDs) are like pointers to sources data can be read or places data can be written. There are three file descriptors:
    * Standart Input (stdin): FD 0
    * Standart Output (stdout): FD 1
    * Standart Error (stderr): FD 2

  * Standart Input is your keyboard basically. Standart Output is where the program returns its output and Standart Error is where the program sends its error messages. Mostly Standart Output and Standart Error directed to your terminal and Standart Input is set to your keyboard by default. But we can redirect them. Does it sounds meaningless? If yes, then you are going to understand what it is with following examples don't worry. Just keep going. These are just definitions, mostly they don't make sense, aren't they? :)

  # Redirection
  * As we discussed earlier, we are able to redirect our file descriptors to different sources and places. 
    * For redirecting Standart Input Stream, we should use the operator **"0<"**. 
    * For redirecting Standart Output Stream, we should use **"1>"**.
    * For redirecting Standart Error Stream, we should use **"2>"**.
  
  * Let's redirect stuff into text files and read inputs from text files. You don't need to create any text file on your desktop. If there is none, commands will create for you. Also you can observe the creation on your graphical interface after you run the commands. 
  * Don't worry about file paths for now. We will discuss about them in detail on later documents. If commands doesnt work because of the path, use **"cd"** command for once and they should work. If you are curious, we are using cd command for navigating through directories. It is short for "change direction". If you don't give any input to cd, it will teleport you into your home directory.

  * Standart Output Example:
    ```
    $ date 1> Desktop/date.txt
    ```
    * Now go inside that text file with your graphical interface or just type "cat Desktop/date.txt" and check what it contains inside. Isn't that exciting?
    * We can also use the ">" operator to direct our input. 

  * Standart Input Example:
    * Let's try to read that file with echo command while redirecting our input from keyboard to text file.
    ```
    $ echo 0< Desktop/date.txt
    ```
    * This should return the content of date.txt file.
    * We can also use the "<" operator to direct our input. 

  * Standart Error Example:
    * For redirecting an error message we should get an error message first, right? So let's do something illegal for Linux Terminal and redirect it with error redirection operator.
    ```
    $ cal imDoingSomethingWrong 2> Desktop/date.txt
    ```
    * Do you remember what cal command were getting as argument? Yes, the date as numbers. So, you should see the error message in date.txt.
    * Did you notice that redirecting output to same text file has overwritten everything in the text file? If you don't want it to overwrite the text file, using "1>>" and "2>>" is going to solve your problem.

    * See you on the next document!