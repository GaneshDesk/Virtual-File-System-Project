# Virtual-File-System-Project
This repo contain Virtual Filesystem project which is based on UNIX like operating system .

---

# Project Name: VFS (Virtual File System) 

---

- #### Technology   : Core C-Programming 
- #### User Interface  : CUI (character User Interface) 
- #### Platform   : Windows NT / Linux 
- #### Hardware Requirements: 20 MB HDD and Processor(any one) 
---

## Introduction :

In this project, we are creating a file system that runs on the primary memory (i.e. RAM). This project is CLI (i.e. Command Line Interface) based. The user interface is Command User Interface. The user interacts with this project by using the following commands.

 #### Commands provided by this project : 

  - ls: Used to list all files in the system.
  - create: Used to create a new file in the system.
  - open: Used to open the file in the system.
  - read: Used to read the existing files in the system.
  - write: Used to write data in the file.
  - truncate: Used to delete data of files in the system.
  - lseek: Used to reposition read/write file offset.
  - close: Used to close the file in the system.
  - closeall: Used to close all open files in the system.
  - stat: Used to display detailed info of files in the system.
  - clear : Used to clear/clean screen/terminal.
  - exit: Used to stop the execution.
  - rm: Used to remove files in the system.

---

## Description :

 - This project provides a UNIX-like filesystem to maintain files & their related information. In UNIX Superblock, UAREA, File Table, Incore Inode Table, DILB, Data Block is used to maintain filesystem structure.
- The superblock contains information about the filesystem as a whole, such as its size (the exact information here depends on the filesystem).
- An inode contains all information about a file, except its name(in our case we store name also). The name is stored in the directory, together with the number of the inode.
- A directory entry consists of a filename and the number of the inode which represents the file. The inode contains the numbers of several data blocks, which are used to store the data in the file.
- Superblock
which contains the information of the inodes that i.e. total number of inodes and number of free inodes. These inodes are created in the DILB block i.e. Data Inode List Block. 
- We created the singly linear linked list of fifty inodes in which each inode has a unique inode number and this inode contains the information of the files which are stored in the data block. 
- The information of each file gets stored in a separate inode that means for a number of inodes we can create a number of files (i.e. for fifty inodes, we can create fifty files).
- When the command prompt opens, the user will have to enter the username and password for the valid authentication. When the user will enter the command, that command will be searched in the program then further operations will happen.
-  When the user will enter some data or text in the file, for that data, the memory gets allocated in the file Buffer and all the text or data will be put in that buffer.
- When the user will read the data giving the size of the bytes, how many data the user wants to read. Then that bytes of data (if exists that number of bytes) will be shown to the user.
- User can write that data up to 1024 bytes (as our file size is 1024 bytes) and can also read the 1024 bytes of data. When a user enters ‘truncate’ command, the data which is stored in the file which contains the text will get erased or gets deleted.
- AT last, when the user hits the 'exit' command then it gets out of the project.

---

## Motivation  :
- Write code in the native language as a C programming.
- Understand the internal working of the UNIX-like operating system.
- Understand Data Structures & their implementation.
---
## Reference  :
- "The Design of the Unix operating system" by  Maurice J. Bach.

---

[Back To The Top](#Virtual-File-System-Project)