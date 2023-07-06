# Basic Shell Permissions

In Linux, permissions control access to files and directories for different users and groups. Permissions are divided into three categories: read, write, and execute.

## Viewing Permissions

To view the permissions of a file or directory, use the `ls -l` command. This will display a long listing of the file or directory, including its permissions.

The permissions are displayed as a series of characters, such as `-rw-r--r--`. The first character indicates the type of file (`-` for a regular file, `d` for a directory). The next nine characters represent the permissions for the user (owner), group, and others, respectively.

Each set of three characters represents the read (`r`), write (`w`), and execute (`x`) permissions. If a permission is not granted, a `-` is displayed instead.

## Changing Permissions

To change the permissions of a file or directory, use the `chmod` command. This command can be used with either symbolic or octal notation to specify the desired permissions.

### Symbolic Notation

In symbolic notation, permissions are represented by letters (`r`, `w`, `x`) and operators (`+`, `-`, `=`). The user, group, and others are represented by `u`, `g`, and `o`, respectively.

For example, to add execute permission for the user (owner) of a file, use the command `chmod u+x filename`.

### Octal Notation

In octal notation, permissions are represented by numbers (`0` to `7`). Each number represents a combination of read (`4`), write (`2`), and execute (`1`) permissions.

For example, to set the permissions of a file to read and write for the user (owner), read for the group, and no permissions for others, use the command `chmod 640 filename.
