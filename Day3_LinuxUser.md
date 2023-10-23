*kali linux* was previously known as backtrack.
vulnerability assessment: - checking a system if it has a vulnerability against a checklist with known vulnerabilities.

penetration testing can be sometimes called ***pro-active*** and ***reactive***.
***pro-active*** is a way of penetration testing in which you test a system before damage happens and generate a report.
***reactive*** is a way of penetration testing after a damage or the system is compromise.

tools in found in kali linux
1. information gathering
2. vulnerability analysis
3. web application analysis
4. data assessment
5. password attacks
6. wireless attacks
7. reverse engineering
8. exploitation tools
9. sniffing and spoofing
10. post exploitation:- used to maintain access after exploiting a system.
11. forensics
12. reporting tools
13. social engineering tools
14. system services
there are usually 2 teams red team and blue team. red are offensive and blue are defensive.

we know linux system uses shell. shell is also called terminal. some distros call is console.
home directory is denoted by ~
local directory with .
all directory *

commands are case sensitive
ls          list directory
ls -l       lists files with detailed info about them including date created, which user created it size of the file(in bytes). 
ls -a      shows all files including hidden files(they have a dot before their name)
ls -R      recursive. opens the folders inside the listed folders.
you can combine the as ls -Rla

cd /     root
cd       home
cd ..     1x back
cd ../..   2x home
cd "folder name" if folder name has space it must be inserted in a double quote

pwd      print working directory
echo     display a line of text/string that are passed as an argument.

echo text > file.txt      writes a text to the file after erasing any existing text(this command doesn't append)
echo text >> file.txt      appends a text to the file

# read from a file
cat      prints the whole text found inside a file onto the screen
head    shows the first lines of the file onto the screen
tail       prints the last lines of the file onto the screen
tail -n    prints the last n number of lines onto the screen
less        prints out the text of a file in a scrollable way unlike the way the command cat does

# creating a file
touch   to create as many files as you want
example: touch geez.md park.txt

# create directory
mkdir
dont forget to insert the folder name in a double quote if it has a whitespace
example: mkdir moonlight "white light" starlight
# clear
clear:      clears your screen 
# remove files
rm: removes files from your computer.
rm -r:        recursive. it is used to delete folders/directories with files as rm can only delete files and empty folders only.
rm -i:     to make the system ask you for a prompt before removing the file
rm -f:      force delete
you can also use them in combination too like rm -rf 'filename'
another example: rm gex.txt light.md

# copy and move files
cp: copy
example 1: cp ../yared.txt .
explanation: copy yared txt file which is found one directory back and paste it in the current working directory
example 2  cp ../yared.txt ../Desktop
explanation: copy yared txt file which is found one directory back and paste it in the Desktop directory which is one directory back from the current working directory

a single dot represents the working directory you are on right now