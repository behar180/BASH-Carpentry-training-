**# BASH-Carpentry-training-
# Bash Carpentry – Day 1 Notes

# What is a Shell?
- A command line  which  interact with your computer
- Allows faster and more powerful control than GUI 

# Accessing the Shell
- Can do in Mac/Linux: Terminal (pre-installed)
- Can also connect to a remote server

# File System Basics
- Files → store data  
- Directories  folders  → store files or other directories  

## Key Commands

### Navigation
- pwd → shows current directory (print working directory)
- ls → lists files/directories
- cd <dir>` → change directory
- cd → go to home directory

### Listing Options
- ls -F → adds `/` to directories
- ls -l → long format (more details)

### Help
- man <command> → opens manual page  
  - q to quit  
  - space = forward, `b` = back  

### Terminal Control
- clear → clears screen  
- `Ctrl + L` → shortcut to clear  

## Important Concepts
- Prompt (`$`) = shell is ready for input  
- Current working directory = where commands run by default  
- / at end of name = directory  

## Tab Completion 
- Press Tab to auto complete file/directory names  
- Saves time and avoids errors  
- Press Tab twice → shows options***

- # Bash Carpentry – Day 2 Notes

## Moving Around the File System

# Going Up a Directory
- `cd ..` → move up one level
- Can chain:
  - `cd ../../` → move up multiple levels

# Viewing Other Directories
- ls <path> → view contents without navigating
- Example:
  - `ls ~/shell_data`

# Absolute Path
- Full location from root (`/`)
- Example:
  ```bash
  cd /home/user/shell_data

  # Bash Carpentry – Day 3 Notes

## Wildcards
- `*` → matches any characters  
- `ls *.fastq` → all FASTQ files  

## Command History
- ↑ / ↓ → scroll commands  
- `history` → list commands  
- `!<number>` → rerun command  
- `Ctrl + R` → search history  

## Viewing Files
- `cat file` → print all  
- `less file` → scroll/search (`q` to quit)  
- `head file` → first lines  
- `tail file` → last lines  
- `-n` → specify number of lines  

## FASTQ Format
- 4 lines per read:
  1. `@` header  
  2. sequence  
  3. `+`  
  4. quality scores  

## File Operations
- `cp` → copy  
- `mv` → move/rename  
- `mkdir` → create directory  
- `rm` → delete (permanent ⚠️)  
- `rm -r` → delete directory  

## Permissions
- `ls -l` → view permissions  
- `chmod -w file` → remove write access 
