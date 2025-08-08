# Customized Virtual File System (CVFS)

## 📌 Project Overview

The **Customized Virtual File System (CVFS)** is a user-defined implementation of a virtual file system in C that replicates core functionalities of the Linux file system. It offers a customized shell that enables file operations like `create`, `read`, `write`, `ls`, `rm`, `open`, `close`, and more.

This system is self-contained and operates independently of the host OS’s native file system, making it ideal for educational purposes and OS-level project demonstrations.

---

## 🛠️ Technology Used

- **Language:** C Programming
- **Platform:** Linux/Windows Terminal (no OS-level file dependency)

---

## 🔍 Features

- Custom shell with built-in commands
- Implements core file system data structures:
  - Incore Inode Table
  - File Table
  - UAREA (User Area)
  - User File Descriptor Table
- Supports Linux-like file operations:
  - `create`, `read`, `write`, `open`, `close`, `ls`, `rm`, `truncate`, `stat`, `fstat`, `lseek`, `man`, etc.
- In-memory management (no actual disk I/O)
- File permission handling (Read, Write, Read+Write)
- Manual (`man`) and help commands built-in

---


## ▶️ How to Run

1. Compile the program:
   ```bash
   gcc -o CVFS.exe CVFS.c
Run the executable:

```bash
./cvfs
```

Use commands like:

```
> help
> man create
> create myfile 3
> write myfile.txt
> read myfile 100
> ls
> stat myfile

```

## 📜 Sample Commands
- create FileName Permission: Create a file
- write FileName: Write content
- read FileName Bytes: Read bytes
- rm FileName: Delete a file
- lseek FileName Offset StartPoint : Move file pointer
- close FileName / closeall : Close files
- stat FileName / fstat FD : Get file info
- help : List commands
- man command : View command manual

## 👩‍💻 Author
Aditi Kishor Yawale
aditikishoryawale@gmail.com
