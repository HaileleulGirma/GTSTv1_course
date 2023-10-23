# awk
used to filter certain characters from a large file
format:    awk '' filename
      or     cat filename | awk
      awk command can also print filtered results.
      example: `awk '{print $0}' example.txt` prints all contents inside the txt file
    if you replace the number zero from above to one it will display the first content on each new line.
    ![[awk1.png]]
if you want to use awk for searching something and print it on screen, then use this format:
`awk '/word_to_be_searched/ {print}'` example.txt
![[awk search.png]]
beware that if you don't explicitly ask for the computer to save the search results it wont save it automatically. to save it just add `> new txt file.txt` so that it will save it on the specified file.

you can display results by from the row you want until the row you want using awk
![[awk NR.png]]
If the field separator is different, you can change the field separator to a character you want. the F in the code below specifies the field separator
![[awk NR.png]]

# sed
is a stream editor for filtering and transforming text. it works like a find and replace tool.
## syntax  `sed 's/FIND/REPLACE/' filename` 
- it still doesn't save unless you order it to.
- by default, it replaces one occurrence of a word in a line. if there are multiple occurrences, you need to add `g` to your sed command.
![[sed1.png]]
- sed can also be used to delete a word/pattern you want, but the syntax for this is a little bit different from the find and replace one. it uses only two slashes.
![[sed delete.png]]
- it can be used to add new lines between data. it still doesn't save it unless you command it.
![[sed newline.png]]
- it can be used to delete empty new lines between data.
- on the photo below, `^` means newline and `$` means end line. so we are commanding the machine to delete empty lines that starts and ends with nothing as there is no word or pattern between our command `^$`. 
![[sed delnewline.png]]

# grep
- it means global search for regular expression and patterns.
- it print lines that match patterns.
#### syntax for search: `grep word filename`
![[grep1.png]]
#### syntax for case-insensitive research: `grep -i word filename`
- it can be used to show on which line the search results are found.
#### syntax for showing the line number: `grep -n word filename`
- it can be used to filter out and delete unwanted word/pattern
#### syntax for filtered delete : `grep -v word filename`
- it can be used to search for a pattern/word recursively (files inside a folder). if you type `.` it will search for it in the local directory.
#### syntax for recursive search: `grep -r word folder`
####  You can combine the options above to reach the desired result.
for example: -rin, -in, -rn, -in etc
![[grep recursive.png]]![[grep c.png]]
