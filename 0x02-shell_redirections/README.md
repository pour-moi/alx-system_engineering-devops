# Shell Redirection

Shell redirection allows you to control where the input and output of a command goes. This can be useful for saving the output of a command to a file, reading input from a file, or chaining multiple commands together.

## Output Redirection

The most common form of shell redirection is output redirection, which allows you to redirect the output of a command to a file. This is done using the `>` operator, followed by the name of the file to save the output to.

For example, to save the output of the `ls` command to a file called `output.txt`, you would use the following command:

Copy
ls > output.txt


This will create a new file called `output.txt` and save the output of the `ls` command to it. If the file already exists, it will be overwritten.

You can also use the `>>` operator to append the output of a command to an existing file, rather than overwriting it. For example, to append the output of the `ls` command to a file called `output.txt`, you would use the following command:

Copy
ls >> output.txt


## Input Redirection

In addition to redirecting the output of a command, you can also redirect its input. This is done using the `<` operator, followed by the name of the file to read input from.

For example, to use the contents of a file called `input.txt` as input for the `cat` command, you would use the following command:

Copy
cat < input.txt


This will read the contents of `input.txt` and pass them as input to the `cat` command.

## Chaining Commands

You can also use shell redirection to chain multiple commands together. This is done using the `|` operator, which takes the output of one command and passes it as input to another command.

For example, to search for all files in the current directory that contain the word "example" and save the results to a file called `results.txt`, you would use the following command:

Copy
grep “example” * | sort > results.txt


This will run the `grep` command to search for all files in the current directory that contain the word "example", then pass its output as input to the `sort` command. The sorted results will then be saved to a file called `results.txt`.

## Conclusion

Shell redirection is a powerful feature that allows you to control where the input and output of a command goes. By using operators like `>`, `<`, and `|`, you can save output to files, read input from files, and chain multiple commands together.
