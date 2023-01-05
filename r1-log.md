# #100DaysOfLinux Log - Round 1 - Charles Gobina

The log of my #100DaysOfLinux challenge. Started on [January 2, Monday, 2023].

## Log

### Round 1 Day 1: January 2

**Today's Progress**: I'm currently in module 5 of NDG Linux Essentials v2 on the Cisco Network Academy. I'm learning about the command line and today, I came across the shell. The Linux Shell is one of the core parts of the linux Operating system and it provides an interface for users to enter commands which tell the kernel what to do. In other words, the linux shell interpretes commands entered in the terminal.
- Bash is the most common shell used in linux. It stands for Bourne Again Shell.

**Command for the day**
- echo $SHELL

### Round 1 Day 2: January 3

**Today's Progress**: 
> The man command
- The primary source of help on how to go about using any command in Linux is by going through the command's manual (man page)
- Other commands like *whatis* and *apropos* will display useful info about some commands too
- It is also important to know where to find these man pages on your system. Commands like *whereis* and *locate* will help with that.
- In addition to the help command, the *info* command can be used to find your way around the OS

> The info command
- The info command provides more and logically related information partaining to a command. It gived you more like a tutorial or cookbook about that command while the man command is more like for reference.

- Man pages are more for quick referencing while info command provides logical and structured documentation.

**Command for the day**
- man ls
- info ls

### Round 1 Day 3: January 4

**Today's Progress**: 
Everything in Linux is considered a file. This is because Linux abstracts everything into a virtual file system
> The Linux File Structure
- At the root of the file system is a directory called the root directory denoted with `/`
- Inside the root directory are other directories which hold files relating to specific things
- For example the dev directory holds files related to your drive.
- The Home directory holds files related to the current user such as Desktop, Downloads, Documents, Picture and Videos.  
- etc

> Navigating the Linux Filesystem
- There are commands that help us navigate this file system
- `ls` to list contents of a directory
- `cd` to change directory
- `pwd` to know current directory
- `pwd` command reveals the the absolute path to our current directory.
- The are two types of path in Linux, *absolute* and *relative* paths
- *Absolute paths* are the full path separated by `/` to our current location. They start from the root of the file system hence always start with `/`
- *Relative paths* is the path to a file or directory separated by `/` from our current location. They always begin with the current directory we are in.

**Command for the day**
- pwd -> display present working directory
- ls / -> list contents of root directory

### Round 1 Day 4: January 5

**Today's Progress**: 
> Globbing
- Glob characters are character with special meaning.
- The are also called wildcard characters and can be used together with any command
- They allow us to specify patterns that match file names, making manipulation of many files possible
- Some of them include
- `*` which represents 0 or more characters
- `?` which represents a single character
- `[]` whcih matches files with any single later contained within the square bracket
- `!` used in conjuction with `[]` and it negates anything found in the square bracket.

> Basic file manipulation commands
`cp` copy files and directories. For it to work, source and destination of item you are copying should be specified. use -i option to make sure you don't mistakenly overwrite a file if it already exists in your destination directory
`mv` renames a file or directory if destination is not provided. The command also moves a file or directory is the destination is provided. use -i option to make sure you don't mistakenly overwrite a file if it already exists in your destination directory
`touch` creates a new file.
`rm` deletes file and directories. To delete directories, specify the -r option else delete won't work on directory. use -i option to make sure you don't mistakenly delete a file or directory as you will be prompted before any deletion is done
`rmdir` deletes a directory but only if it is empty
`mkdir` creates a directory

**Command for the day**
- touch the_sky -> creates a file called the_sky
- rm the_sky -> deletes a file called the_sky
