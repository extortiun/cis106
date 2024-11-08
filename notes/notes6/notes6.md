# Note 6: Wildcards

## *
### Definition:
The main wildcard is a star or asterisk (*) character. A star alone matches anything and nothing and matches any number of characters.
### Examples:
* `ls *.txt`
* `ls ~/Downloads/*.png`
* `ls file.*`

<hr>

## ?
### Definition:
The ? wildcard meta character matches precisely one character. The ? wildcard proves useful when working with hidden files (*hidden files are also called* **dot files**).
### Examples:
* `ls .??*`
* `ls ./.??*`
* `ls ~/Downloads/f?ll.sh`

<hr>

## []
### Definition:
The brackets wildcard match a single character in a range. The brackets wildcard use the exclamation mark to reverse the match. 
### Examples:
* `ls f[aeiou]*`
* `ls ~/Downloads/f[0-9]ll.sh`
* `ls f[a-z]*`
* `ls *[0-9]*`

<hr>

## {}
### Definition:
Brace expansion {} is not a wildcard but another feature of bash that allows you to generate arbitrary strings to use the commands.
### Examples:
* `touch website{1..5}.html`
* `touch file{A..Z}.txt`
* `touch file{001..10}.py`