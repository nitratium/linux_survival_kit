*** GRAMMER CHECK

# Pipelines
 * Linux commands are designed to do one thing and do it in the most efficient way. But a limitation comes out here. What if we want to handle more than one thing in only one execute? Well, the true power of the linux command line comes out with a feature named piping. 
 * We can chain our commands to work together. In definition, we are connecting the standard output of one command to the standard input of anouther command. We are using the operator "|" to pipe our commands. (For english keyboards it's Shift + Backslash, for Turkish Q keyboards it is Alt Gr + < (next to Z))

 Example:
 ```
 $ first_command –options arguments | second_command -options arguments
 ```
 * Piping can be extended as long as you want.

 # tee Command
 * Redirecting during a pipeline causes the pipeline to break. For example, the command below won't work.
  ```
  $ first_command –options arguments > text.txt | second_command –options arguments
  ```
 * If we want to redirect an output to a file and add new commands to pipeline, we should use **"tee"** command. Let me show you how it works.
  ```
  $ first_command –options arguments | tee text.txt | second_command –options arguments
  ```
 * This should do the trick. This command takes the first commands output and prints that to text.txt and gives it to second command as input.

 # xargs
 * There are some commands that only accept command line arguments. **(e.g. "echo" command)**
 * echo command only accepts command line arguments. So we need something to switch our first command's structure from standard output to command line argument. Here is where **xargs** helps us.
  ```
  $ first_command –options arguments | echo
  ```
  * This won't work! As we said earlier, echo command needs an command line argument.

  ```
  $ first_command –options arguments | xargs echo
  ```
  * This will work. xargs transforms the data to command line arguments which is coming from first command.