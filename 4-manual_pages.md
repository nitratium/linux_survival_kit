
# Manual Pages
 * So, we learned the command structure and some basic commands with some of their options. But you might be asking "This was just a start how am I supposed to know all of it?". Well, yes you are right. Most of us won't be able to memorise all of the commands and these command's every option. This is why we have something called **Manual Pages**.

 * Manual pages are structured in 8 sections.
  1. A
  2. B
  3. C

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

 # help Command
 * Some commands may not have a manual page. There is also a help command that gives us a little information about some commands.
 ```
 $ help <commandName>
 ```
 * This works too similar to man command. Don't forget to give it a try!