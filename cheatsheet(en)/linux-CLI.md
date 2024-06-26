# cheatsheet terminal

### File System Navigation  
- `ls` Lists files and directories in the current directory.
    - `-l` Long listing format, displaying additional information about files.
    - `-a` Include hidden files (those starting with a dot).
    - `-h` Display file sizes in human-readable format.
    - `-t` Sort files by modification time.
    - `-r` Reverse the order of the sort.
    - `-R` Recursively list subdirectories encountered.
- `cd [directory_name]` Changes the working directory.
- `pwd` Prints the path of the current directory.
- `cat [file_name]` Display file contents.
- `less [file_name]` View file contents one page at a time.
    - `Spacebar` Move forward one page.
    - `b` Move backward one page.
    - `/pattern` Search forward for the next occurrence of pattern.
    - `?pattern` Search backward for the previous occurrence of pattern.
    - `q` Quit less.
- `head [file_name]` Display the first few lines of a file.
    - `-n [num]` Display the first [num] lines of the file.
- `tail [file_name]` Display the last few lines of a file.
    - `-n [num]` Display the last [num] lines of the file.
    - `-f` Output appended data as the file grows (tail -f
- `grep [pattern] [file_name]` Search for a pattern in a file.
    - `-i` Ignore case distinctions in both the pattern and input files.
    - `-v` Invert the match, selecting non-matching lines.
    - `-n` Prefix each line of output with the 1-based line number within its input file.
    - `-r` Recursively search subdirectories listed.

### File Manipulation

- `touch [file_name]` Creates a new empty file.
- `nano [file_name]` Opens the file in the Nano text editor.
- `mkdir [directory_name]` Creates a new directory.
- `rm [file_name]` Deletes a file.
    - `-rf ` Deletes all child of this file or directory
- `rmdir [directory_name]` Deletes an empty directory.
- `cp [source] [destination]` Copies files or directories.
    - `-r` Recursively copies directories and their contents.
- `mv [source] [destination]` Moves or renames files or directories.
### Permission Management

- `chmod [permissions] [file_name]` Changes the permissions of a file or directory.
    - `-R` Recursively change permissions of directories and their contents.
- `chown [user:group] [file_name]` Changes the owner and/or group of a  file or directory.
    - `-R` Recursively change ownership of directories and their contents.
- `chgrp group file/directory` This command is used to change the group ownership of a file or directory.  
    - `-R` Recursively change group ownership of directories and their contents.
### Processes and System

- `ps` Displays active processes.
    - `-e` Display information about all processes.
    - `-f` Display a full listing.
    - `-u user` Display processes owned by a specific user.
    - `aux` Display a detailed listing of all processes.
- `kill [PID]` Kills a process using its Process ID (PID).
    - `9` Forcefully terminate the process.
- `top` Displays running processes and their resources.
    - `q` Quit top.
    - `k` Kill a process.
    - `u` Specify user.
    - `H` Toggle threads display.
    - `P` Sort by CPU usage.
    - `M` Sort by memory usage.
    - `R` Reverse the sorting order.
- `pgrep pattern` This command is used to search for processes by name and other attributes. 
    - `-l` Display process names as well as PIDs.

### Archives and Compression

- `tar -cvf [archive_name.tar] [files]` Creates a tar archive.
    - `-c` Create a new archive.
    - `-v` Verbose mode, shows files being archived.
    - `-f [archive_name.tar]` Specifies the archive filename.
- `tar -xvf [archive_name.tar]` Extracts a tar archive.
    - `-x` Extract files from an archive.
    - `-v` Verbose mode, shows files being extracted.
    - `-f [archive_name.tar]` Specifies the archive filename.
- `gzip [file_name]` Compresses a file using gzip.
- `gunzip [file_name.gz]` Decompresses a gzip file.

### Networking

- `ping [ip_address_or_domain_name]` Checks network connectivity.
- `ifconfig` Displays information about network interfaces.
- `ssh [user@ip_address]` Connects to a remote machine via SSH.
    - `-p` Add a port to the adress
	- `-l` Login name
- `scp [file] [user@ip_address:destination]` Copies files via SSH.

Help and Documentation

- `man [command]` Displays the manual for a specific command.
    - `--help` Add this to a command to display quick help.