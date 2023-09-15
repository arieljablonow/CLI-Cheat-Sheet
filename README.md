# CLI Cheat Sheet

Linux commands

## Directory Traversal

`cd dir` 
naviate to dir

`cd dir1/dir1/dir3` 
navigate to dir3

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
list content + file info

`cd dir && ls`
navigate to dir and list content 

`mkdir <name>` create a directory 

`rm file.txt` removes file 

## Files
`echo > file.txt` create a file if the file does not already exist

`echo text > file.txt` if file.txt already exists, this command will overwrite file.txt with 'text'

`echo text >> file.txt` append text to file.txt

Important: <br />
`>` OVERRIDE
`>>` APPEND

`cat file.txt` display content of file

`head file.txt` dispay first ten lines of file

`head -n x file.txt` display the first x lines of file

`tail state.txt` display last ten lines of file

`tail -n x state.txt` display last x lines of file 

### permissions
Three sets of permissions - owner, user group, everyone else <br />
When file permissions are displayed, it goes owner|group|everyone else
`u` user <br />
`g` group <br />
`o` other <br />

example - <br />
`rwxrw-r--` 
+ owner can read, write, and execute
+ group can read and write
+ everyone else can read

Number representation: <br />
`4` - read <br />
`2` - write <br />
`1` - execute <br />

When permissions are represented by numbers the first digit is for the user, second digit is for the group, third is for everyone else

example - <br />
`764`
+ owner can read, write, and execute 
+ group can read and write 
+ everyone else can write 

`chmod` command used to make changes to permission


## Network
`ifconfig` displays current network interface configurations  
This will include:

+ IPv4 addresses
+ IPv6 addresses
+ MAC addresses associated with those interfaces
+ Connection speeds
+ Network masks
+ Broadcast domains 
+ Other confiiguration details 

`ifconfig` can also be used to enable and disable itnerfaces, refresh or drop DHCP packets, and control the network interfaces
    
`ping` test functionality, confirm a connection between two hosts 

`traceroute <destination>` outputs path taken from source to destination 

`curl` used to transfer data via URLs <br />
Can also be used for file transfer via FTP, FTPS, SFTP 

`arp` provides information about the local host's ARP cache

`route` will display and modify a system's routing tables



### netstat 
USED FOR: getting information about active connections <br />
`netstat` provides network statistics by protocol. For every connection, it will include information about the local address and remote address. It also provides information about the state of TCP connections.

### netcat 
USED FOR: creating network connections, transferring data <br />
Known as the Swiss army knife because it is very versatile. <br />
Basic command: `nc <hostname> <port>` <br />
netcat can act as a client and a listener

### nmap
USED FOR: host profiling <br />
`nmap` is a port scanning tool <br />
It can scan for:
+ Hosts 
+ Services and service versions
+ Operating systems

Command: `nmap <IP address or hostname>`

### important ports

7 echo 

20 FTP transfer

21 FTP connection 

22 SSH 

23 telnet 

25 SMTP 

53 DNS 

80 HTTP 

88 Kerberos 

110 POP3 

149 IMAP 

389 LDAP 

443 HTTPS

636 LDAPS 

990 FTPS 

993 IMAPS 

995 secure POP 

1812, 1813 RADIUS 

3389 remote desktop protocol 

## Other
`dd` used to create images for forensic or other purposes <br />
Used to create a bit by bit copy of a drive - hence why it's used for many forensic tools<br />
Command takes an input location  - `if` and an output location - `of` <br />
Can create a disk image or restore from an image 

`memdump` copy information in system memory to the standard output stream 

`dig` DNS queries, can determine the IP addresses associated with domain names 

`nslookup` simpler version of `dig`

`whois` provide information about the registered owners of domain names 

`dnsenum` dns deep dive - generates detailed recon info




