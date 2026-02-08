# Linux Basic Commands Inference - Yadu Krishnan.S

This document records my observations and inferences while executing fundamental Linux commands in the terminal.

---

### 1. Setup and Directory Creation
* `mkdir ev4` : Created a new directory named 'ev4'.
* `cd ev4` : Changed current directory to 'ev4'.
    * **Resultant Path:** `/home/yadu/ev4`
* `mkdir 64` : Created a directory named '64' (my roll number).
* `cd 64` : Entered the directory '64'.
    * **Resultant Path:** `/home/yadu/ev4/64`

### 2. Navigation Commands
* `cd -` : Switched back to the previous directory (`ev4`).
* `cd ..` : Moved up one level to the parent directory.
* `cd ~` : Moved immediately to my Home directory.
* `pwd` : Printed the absolute path of the current directory.
    * **Output:** `/home/yadu`
* `cd /media` : Successfully entered media using an absolute path.

### 3. File and Directory Management
* `touch file1` : Created an empty file named 'file1'.
* `rm -i file2` : Deleted 'file2' after interactive confirmation.
* `rmdir emptydummy` : Successfully removed a directory because it was empty.
* `rm -r dummy` : Recursively removed a directory and all the files inside it.

### 4. File Content and Redirection (I/O)
* `cat > file1.txt` : Created a file and allowed text input.
* `cat file1.txt file2.txt > file_combined.txt` : Combined two files into a new one.
* `cat file3.txt >> file_combined.txt` : Appended new content to the end of an existing file.
* `grep -i hello file*` : Filtered and listed lines containing "hello" from all files.
* `mv file_combined.txt combined` : Renamed the file to 'combined'.

### 5. Permissions (chmod)
* `chmod u+x combined` : Added execute permission for the owner.
* `chmod g-r combined` : Removed read permission for the group.
* `chmod 777 combined` : Granted full read, write, and execute access to everyone.

### 6. User Management (sudo)
* `sudo useradd alice` : Created a new system user named 'alice'.
* `sudo userdel alice` : Deleted the user account 'alice' from the system.

### 7. Communication
* `write alice` : Sent a real-time message to another user's terminal.
* `mesg n` : Disabled the ability to receive messages from others.

---
**Summary:** These commands demonstrate the core capabilities of the Linux Shell for user management, security, and file system navigation.
