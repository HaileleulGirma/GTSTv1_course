![[wc.png]]
#### multiple command execution
you can run/execute multiple commands in one line using 3 methods.
1. and (&&)
2. or ( || )
3. piping ( | )

### 1. and
- executes multiple commands if all of them are successful. it means that if one of the commands fail to be executed, the rest won't be executed.
eg: `touch day4.md && echo "this is my document."` will execute and print the text on the screen, but `toch day4.md && "this is my document."` won't be executed because 'u' is missing in touch and because we are using and as a multi-line(aka multiple command execution tool) the text won't be printed on the screen.
### 2. or
- using or as a multi-line, if one command fails to execute, it won't affect the execution of the rest of the commands written.
- if we take take the command `toch day4.md && echo "this is my document."` the echo command will be executed even if the 'u' in touch is missing and the text will be printed on the screen.
### 3. piping
this command will help us run commands by using the output of the first command as the input for the next one.

eg: `cat example.txt| grep "hello"` this command using piping allows us to use the output of the first command and search for the desired word 'hello'.
file system is a directory structure that the OS uses.
system files are files that are used by the system OS.
while the windows system file appear under the local disk C:, linux system files appear under the root directory ( / ).

- the `/sbin` directory **contains binary executables and command line tools that are preserved for the root user**.
### /(root)
- every single file and directory starts from the root directory.
- only the root user has the right to write under this directory.
- /root is the root user's home directory, which is not the same as /
![[vim def.png]]
![[openinf vim.png]]
![[opening insert vim.png]]
pressing tab while writing a command can auto-complete the command for you(if the command you are writing is correct of course)
creating users using useradd is simple yet lacks
- home folder with the user's name
- no password during login
- uses shell instead of bash(if created using adduser)
to exit from root user to normal user, type `exit` and enter.