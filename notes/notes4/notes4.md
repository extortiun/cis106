# Notes 4: The Linux FS

## Each of the commands used for navigating the file system

## File System
### Definition:
The way files are stored and organized. 
### Usage:
Directory and folder mean the same thing. First directory in the file system is called the root directory. Filesystem Hierarchy Standard (FHS) specifies requirements and guidelines for file and directory placement UNIX-like operating systems. 

<hr>

## pathname
### Definition: 
In a filesystem, every file has a pathname which indicates the location of the file in the filesystem. 
### Examples:
* ./ = current directory.
* ../ = the parent directory.

<hr>

## Absolute path
### Definition:
the location of a file starting a the root of the file system.
### Example: 
* `/home/john/Downloads/songs.mp3`
* `/people2/Mary`

<hr>

## Relative path
### Definition:
the location of a file system starting from the current working directory or a directory that is located inside the current working directory.
### Examples:
* `Downloads/song.mp3`
* `../people2/Mary`
* `projects/dataset1`

<hr>

## Difference between YOUR HOME and THE HOME directory
### Definition:
Both $HOME and ~ point to the same folder, the current user's home folder, but both are very different things. $HOME is an environment variable that is set to the contain the home folder of the current user. ~ is a shell expansion symbol. 
### Examples:
* `$ echo ~`
* `/home/elias`
* `$ echo ~/.ssh`

<hr>

## parent directory
### Definition:
a named group of files (a folder); a  directory that contains more folders are called the "parent".
### Examples:
* `cd ..`
* `cd ../../`

<hr>

## child directory
### Definition:
the folder within it is referred to as the "child" of the directory. 
### Examples:
* `pwd /home/dude/`
* `cd a/b/*/.`
* `cd a/b/*/./c`

<hr>

## Bash special characters
### Definition:
Tab completion - auto completes a command by pressing the tab key. Arrow keys allows you to move, edit, and repeat commands. 
### Examples:
* `Ctrl + a` - go to the start of the command line
* `Ctrl + e` - go to the end of the command line

<hr>

## environment variables
### Definition:
environment variables are used by the shell to track specific system information and user information.
### Usage:
`env`+`set`+`printenv`
### Examples:
* `echo $USER` will display the current user
* `echo $SHELL`
* `echo $PATH`
  
<hr>

## user variables
### Definition
User variables are created by the user and exist only in the script and subshell that runs the script. 
### Usage:
`letters`+`digits`+`underscore characters`
### Examples:
* `name='Peter'`
* `age='45'`

<hr>

## Why do we need to use $ with variables in bash shell scripting?
### Answer
The shell stores the PID number of the process that is executing it in the '$$' variable. Shell stores the exit status of the last command in the '$?' variable, non-zero exit means that the command failed. 