
# Manual Pages
 * So, we learned the command structure and some basic commands with some of their options. But you might be asking "This was just a start how am I supposed to know all of it?". Well, yes you are right. Most of us won't be able to memorise all of the commands and these command's every option. This is why we have something called **Manual Pages**.

 * Manual pages are structured in 8 sections.
   1. User Commands
     * These are the commands that can be run from the terminal by any regular user.
   2. System Calls
     * 
   3. Library Functions
     * 
   4. Devices
     * 
   5. Files
     * 
   6. Games
     * 
   7. Miscellaneous
     * 
   8. System Administration
     * 

 * Linux has manual pages for most of the commands. With "man" command we are able to look into manual page for a spesific command.

 ```
 $ man <commandName>
 ```

 * This command will open manual page for the name you have given.

 * If we want to find a new command for a usage, we can search through manual pages with -k option.

 ```
 $ man -k <search term>
 ```

 * This will return the commands containing the search term in its name or description.

 * In addition when you open a manual page, the text is being displayed on a new page on your terminal. To exit that screen you need to click **q**. With this feature, a large line of text on any manual page will not fill your terminal.


 # help Command
 * Some commands may not have a manual page. There is also a help command that gives us a little information about some commands.
 ```
 $ help <commandName>
 ```
 * This works too similar to man command. Don't forget to give it a try!