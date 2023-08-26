# CLI Cheat Sheet

## Directory Traversal

`cd dir` 
naviate to dir

`cd dir1/dir1/dir3` 
navigate to dir3

`cd -` 
go back one level 

`cd ~` 
go to home directory 

`cd ..` 
return to parent directory

`cd -`
return to previous working directory 

`cd "my dir"`
navigate to a dir with a space in the name

`pwd` 
get current file path

`ls`
list content of current directory 

`ls -a`
list content including hidden files

`ls -l `
lsit content + file info

`cd dir && ls`
navigate to dir and list content 

## Files
`echo > file.txt` create a file if the file does not already exist

`echo text > file.txt` if file.txt already exists, this command will overwrite file.txt with 'text'

`echo text >> file.txt` append text to file.txt

Important: <br />
`>` OVERRIDE
`>>` APPEND

`cat file.txt` display content of file

## Network
`ifconfig` displays current network interface configurations  

`ping` test functionality, confirm a connection between two hosts 






