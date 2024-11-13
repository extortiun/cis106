# Note 7: Handling Text Files

Commands cover in lecture: 

## Cat
### Definition:
The cat command is used for displaying the content of a file. Cat is short for concatenate which is the command's intended use. 
### Usage:
`cat`+`option`+`file(s) to display`
### Examples:
* Display the content of a file located in the pwd
  * `cat todo.lst`
* Display the content of a file using absolute path
  * `cat ~/Documents/todo.lst`
* Display the content of a file with line numbers
  * `cat -n ~/Documents/todo.md`
* Display the content of a file with line numbers excluding empty lines
  * `cat -b ~/Documents/todo.md`

<hr>

## tac
### Definition: 
The tac command is used displaying the content of a file in reverse order. Just like cat, tac concatenates files and displays the output of the concatenation
### Usage:
`tac`+`option`+`file(s) to display`
### Examples:
* Display the content of a file located in the pwd
  * `tac todo.md`
* Display the content of a file using absolute path
  * `tac ~/Documents/todo.md`

<hr>

## head
### Definition:
The head command displays the top N number of lines of a given file. By Default, it prints the first 10 lines. If more than one file name is provided then data from each file is preceded by its file name. 
### Usage:
`head`+`option`+`file(s)`
### Examples:
* Display the first 10 lines of a file
  * `head ~/Documents/Book/dracula.txt`
* Display the first 5 lines of a file
  * `head -5 ~/Documents/Book/dracula.txt`
* Display the first 5 lines of multiple files
  * `head -n 5 dracula.txt bible.txt war-and-peace.txt`
* Display the first line of multiple files using wildcards
  * `head -n 1 *.csv *.py`
* Display the name of the file in the output
  * `head -v -n 7 ~/Documents/Books/dracula.txt`

<hr>

## tail
### Definition:
The tail command displays the last N number of lines of a given file. By default, it prints the first 10 lines. If more than one file name is provided then data from each file is preceded by its file name. 
### Usage:
`tail`+`option`+`file`
### Examples:
* Display the last 10 lines of a file
  * `tail ~/Documents/Book/dracula.txt`
* Display the last 5 lines of a file
  * `tail -5 ~/Documents/Book/dracula.txt`
* Display the last 5 lines of multiple files
  * `tail -n 5 dracula.txt bible.txt war-and-peace.txt`

<hr>

## cut
### Definition:
The cut command is used to extract a specific section of each line of a file and display it to the screen.
### Usage:
`cut`+`option`+`file(s)`
### Examples:
* Display a list of all the users in your system
  * `cut -d ':' -f1 /etc/passwd`
* Display a list of all the users in your system with their login shell
  * `cut -d ':' -f1,7 /etc/passwd`
* Cut a range of bytes per line
  * `cut -b 1-5 usernames.txt`
* Cut a file excluding a given field
  * `cut -d ',' --complement -s -f3 users.txt`

<hr>

## sort
### Definition:
Tne sort command is used for sorting files. The sort command supports sorting: alphabetically, in reverse order, by number, and by month.
### Usage:
`sort`+`option`+`file`
### Examples:
* Sort a file
  * `sort users.lst`
* Sort a file and save the output to a new file
  * `sort -o sorted.lst users.lst`
* Sort a file in reverse order
  * `sort -r users.txt`
* Sort by column number
  * `sort -k 2 users.txt`

<hr>

## wc
### Definition:
The wc command is used for printing the number of lines, characters and bytes in a file.
### Usage:
`wc`+`option`+`file(s)`
### Examples:
* Display the number of characters in a file
  * `wc -m users.txt`
* Display the number of lines in a file
  * `wc -t users.txt`
* Display the number words in a file
  * `wc -w users.txt`

<hr>

## tr
### Definition:
The tr command is used for translating or deleting characters from standard output. 
### Usage:
`Standard` | `tr`+`option`+`set`+`set`
### Examples:
* Translate one character to another comma.
  * `cat file.txt | tr '.' ','`
* Translate white space into tabs.
  * `cat program.py | tr "[:space:]" '\t'`
* Translate tabs into space.
  * `cat file.py | tr -s "[:space:]" ' '`
  
<hr>

## diff
### Definition:
Tne diff command compares files and displays the differences between them.
### Usage:
`diff`+`option`+`file1`+`file2`
### Examples:
* Display the difference between two files
  * `diff cars.csv cars-backup.csv`
* Display the difference between two files in a column format:
  * `diff -y cars.csv cars-backup.csv`

<hr>

## grep
### Definition:
Grep is used to search text in given file. Grep works line by line basis. 
### Usage:
`grep`+`option`+`search criteria`+`file(s)`
### Examples:
* Search any line that contains the word "dracula" in the given file:
  * `grep 'dracula' ~/Documents/dracula.txt`
* Search any line that contains the word 'dracula' regardless of the case
  * `grep -i 'dracula' ~/Documents/Books/dracula.txt`
* Search any line that contains the word dracula regardless of case and with number line
  * `grep -in 'dracula' ~/Documents/Books/dracula.txt`
* Search for all lines that do not contain the word 'war'
  * `grep -v 'war' ~/Documents/Books/war-and-peace.txt`
* Display how many lines contain the matched string
  * `grep -c 'dracula' ~/Documents/Books/dracula.txt`
* Search for a given strings inside file in a given directory
  * `grep -iR 'conf' /etc/`
* Search for all lines that start with a capital letter
  * `grep -n '^[A-Z] ~/Documents/Books/war-and-peace.txt`
* Search for more than one word per line
  * `grep -Ewn 'horror|love|scare' ~/Documents/Books/dracula.txt`