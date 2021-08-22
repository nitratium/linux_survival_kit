# Pipelines
 * Linux commands are designed to do one thing and do it in the most efficient way. But a limitation comes out here. What if we want to handle more than one thing in only one execute? Well, the true power of the linux command line comes out with a feature named piping. 
 * We can chain our commands to work together. In definition, we are connecting the standard output of one command to the standard input of anouther command. We are using the operator "|" to pipe our commands. (For english keyboards it's Shift + Backslash, for Turkish Q keyboards it is Alt Gr + < (next to Z))

 Example:
 ```
 $ first_command –options arguments | second_command -options arguments
 ```
 * Piping can be extended as long as you want.

 # tee Command

 # xargs