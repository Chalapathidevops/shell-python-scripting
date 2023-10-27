## 1. List some of the commonly used shell commands
**man:** command is used to display the manual pages for various Unix/Linux commands. Ex: `man ls`

**<ins>File and Directory Management:<ins>**

**ls:** List files and directories.<br>
**cd:** Change the current directory.<br>
**pwd:** Print the current working directory.<br>
**touch:** Create an empty file.<br>
**mkdir:** Create a new directory.<br>
**rmdir:** Remove an empty directory.<br>
**rm:** Remove files or directories.<br>
**cp:** Copy files or directories.<br>
**mv:** Move or rename files or directories.

**<ins>File Viewing and Editing:<ins>**

**cat:** Concatenate and display file content.

**more** or **less:** Paginate through file content.<br>
**head:** Display the beginning of a file.<br>
**tail:** Display the end of a file.<br>
**nano, vim, or emacs:** Text editors for editing files.

**<ins>File Search and Text Processing:<ins>**

**find:** Search for files and directories.<br>
**sed:** Stream editor for text manipulation.<br>
**awk:** Text processing tool for data extraction.

**<ins>File Permissions:<ins>**

**chmod:** Change file permissions.<br>

**chown:** Change file ownership.<br>
**chgrp:** Change group ownership.

**<ins>Archiving and Compression:<ins>**

**tar:** Archive files and directories.<br>

**gzip, gunzip, bzip2, unzip:** Compress and decompress files.

**<ins>User and Group Management:<ins>**

**useradd** and **userdel:** Create and delete user accounts.

**passwd:** Change user passwords.<br>
**groups:** Display user group memberships.

**<ins>Process Management:<ins>**

**ps:** List running processes.

**top** or **htop:** Real-time system monitoring.
**kill:** Terminate processes.
**nohup:** Run a command immune to hang-ups.

**<ins>System Information:<ins>**

**uname:** Display system information.

**df:** Display disk space usage.<br>
**free:** Display memory usage.

**<ins>Networking:<ins>**

**ifconfig** or **ip:** Network interface configuration.

**ping:** Test network connectivity.
**netstat** or **ss:** Network statistics.
**ssh:** Secure Shell for remote access.

**<ins>Package Management (Linux):<ins>**

**apt** (Debian/Ubuntu), **yum** (Red Hat/CentOS), or **dnf** (Fedora): Package management commands for installing, updating, and managing software.


## 2. Write a simple shell script to list all processes IDs
```bash
#!/bin/bash

# Use the ps command to list all processes and extract PIDs
pids=$(ps -ef | awk '{print $2}')

# Display the extracted PIDs
echo "PIDs of running processes:"
echo "$pids"
```



## Pending...
3)write a script to print only errors from a remote log
  curl google.com | grep   

4)write a shell script to print numbers divided by 3 & 5 and not 15
  
5)write a script to print number of "s" in mississippi
  grep -o "s" <<<"$x" | wc -l 
6)How will you debug the shell script
 set -x => set debug mode
7) what is crontab in linux? can you provide and example of usage
8) How to open a read-only file
   vi -r test.txt
9) what is the difference between soft and hadr link
10)what is the diff between break and continue statement
11)what are some disadvantages of shell script
12)what are the diff types of loops and when to use
13)is bash dynamic or stattically yped and why
14)explain about a network troubleshooting utility
  traceroute is a tool, we are using for tracig   
  ex: traceroute google.com
15)how will you sort list of names in a file
  sort command
16) how will you manage logs of a system that generate huge files everyday
  using logrotate
  
