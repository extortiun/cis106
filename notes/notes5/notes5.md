# Note 5: Managing Files

## mkdir
### Definition:
is a command-line utility that allows users to create new directories. 
### Examples:
* `mkdir wallpapers`
* `mkdir wallpapers/ocean`
* `mkdir ~/wallpapers/forest`

<hr>

## Touch
### Definition:
can be used to create files. 
### Examples:
* `touch list`
* `touch list_of_cars.txt script.py names.csv`
* `touch ~/Downloads/games.txt`
* `touch Downloads/games2.txt`

<hr>

## rm
### Definition:
Removes files. RM by default does not removes directories. To remove a directory use rm with the -r option. 
### Examples:
* `rm list`
* `rm -i list`
* `rm -r Downloads/games`

<hr>

## rmdir
### Definition:
used to remove directories. 
### Examples: 
* `rmdir Downloads/games`

<hr>

## mv
### Definition:
moves and renames directories.
### Usage: 
* `mv`+`source`+`destination`
* `mv`+`file/directory to rename`+`new name`
### Examples:
* `mv Downloads/homework.pdf Documents/`
* `mv Downloads/english_homework.docsx /media/student/flashdrive/`
* `mv homework.docx cis106homework.docx`
* `mv ~/Downloads/homework.docx ~/Downloads/cis106homework.docx`
* `mv Downloads/cis106homework.docx Documents/new_cis106homework.docx`

<hr>

## cp
### Definition:
copies files and directories from a source to a destination. 
### Usage:
* `cp`+`files to copy`+`destination`
* `cp -r`+`directory to copy`+`destination`
### Examples:
* `cp Downloads/wallpapers.zip Pictures/`
* `cp -r ~/Downloads/wallpapers ~/Pictures/`
* `cp Downloads/wallpapers/* ~/Pictures/`

<hr>

## file
### Definition:
determines the file type of a file.
### Examples
* `file filename`
* `file -b filename`

<hr>

## pdfinfo
### Definition:
displays information about pdf files
### Examples:
* `pdfinfo filename.pdf`

<hr>

## mediainfo
### Definition:
command line utility to display information about audio/video files.
### Examples:
display information about a media file
* `mediainfo example.png`
display full information of a media file
* `mediainfo -f example.png`
Output information to an html file
* `mediainfo --output=HTML example.png > file.html`

<hr>

## exiv2
### Definition:
image metadata manipulation tool
### Usage:
* `exiv2`+`[option][action][file]`
### Examples:
Displays information about an image file
* `exiv2 example.png`
Displays all exif data about an image file
* `exiv2 -pt example.png`

<hr>

## exiftool
### Definition:
Read and write meta information in files
### Usage:
see man page
### Examples:
Displays information about a file
* `exiftool example.png`