# Training Day :- 02

Day two of the summer training program was about the study of booting in linux.

## What is Booting?
Booting is the process of starting a computer. When you switch on your computer, the system loads the operating system (like Windows or Linux) from the hard drive into the RAM (memory), so you can use the computer.
###  Booting Process :
- ***Power On*** – You turn on the computer.
 
- ***POST (Power-On Self-Test)*** – System checks hardware (RAM, keyboard, etc.).
 
- ***BIOS/UEFI Loads*** – Basic system firmware starts.

- ***Boot Loader Activated*** – BIOS/UEFI finds and runs the boot loader.

- ***OS Loading*** – Boot loader loads the operating system into RAM.

- ***System Ready*** – Operating system starts, and the computer is ready to use.

## Types of Booting:
#### Cold Booting (Hard Booting):
Happens when the computer is started from the power-off state.
Example: You press the power button to turn on your PC.
### Warm Booting (Soft Booting):
Happens when the system restarts without turning off the power.
Example: You click Restart or press Ctrl + Alt + Del.

### Structure of Linux shell
![image](https://github.com/user-attachments/assets/ca35c78f-f999-4a0a-b5ed-422d5e888218)


### Study of Kernel
The kernel is the core part of an operating system.It manages the communication between hardware and softwar
it also manages Memory management,File manangement,Device management,Process managementetc.

###  study of Shell
The shell is a program that acts as an interface between the user and the operating system.It takes user commands and tells the operating system to perform tasks.

### Types of Shell
Shells are mainly divided into two categories:
### 1. Command-Line Interface (CLI) Shells
User interacts by typing commands. Fast and powerful for developers and system admins
### Types of CLI Shells
|shell name | description| 
|-----------|------------|
|**sh**|bourne shell(original unix shell)|
|**bash**|bourne again shell(most popular shell)|
|**csh**|c shell(c like syntax)|
|**ksh**|korn shell(advanced features)|
|**zsh**|z shell(user friendly & customizable)|

From these CLI shells , **BASH** is the most important shell.
### 🐚 What is **Bash**?

**Bash** stands for **Bourne Again SHell**.
It is a **command-line shell** used in **Linux** to **interact with the operating system**.> **Bash** is a program that lets you **type commands** to control your computer without using the mouse.
* Used to **run commands** like creating files, copying, moving, or deleting.
* Supports **scripting**, so you can **automate tasks** with `.sh` files.
* Built-in on **Linux**, **macOS**, and available for **Windows** (via WSL or Git Bash).

---

### **Example Bash Commands:**

```bash
ls       # list files
cd       # change directory
mkdir    # make a new folder
rm       # remove files/folders
echo     # print text
```

---

### **Example of a Bash Script:**

```bash
#!/bin/bash
echo "Hello, Kiran!"
mkdir my_folder
cd my_folder
touch file.txt
```

---

### ** Importance of BASH in linux:**

* Core part of **Linux system administration**.
* Helps in **automation** (via shell scripting).
* Essential for **DevOps**, **ethical hacking**, **software development**, and more.

---

### 3. Graphical User Interface (GUI) Shells
User interacts using windows, icons, and buttons.Easy for beginners.Example : GNOME, KDE (on Linux)

### Linux File System Structure
The Linux file system starts from the root directory /.
All files and folders are inside this root, even if they are on different drives.
![image](https://github.com/user-attachments/assets/285090b7-04cc-42f5-9da7-0855a8f1d808)



### Main Folders in Linux File System
|Directory	|        Meaning|
|-----------|---------------|
|**/** |	Rootof everything.|
|/home|Personal folders for users (like /home/kiran)|
|/lib	|Shared libraries for programs|
|/bin	|Essential binaries (like ls, cp, etc.)|
|/boot	|Files needed to boot the system|
|/dev |device files,hardware files,device files etc.|
|/media	|Used to mount USB drives, CDs etc.|
|/mnt  |same as media.|
|/opt	|Optional software packages|
|/sbin	|System admin commands|
|/tmp	|Temporary files (auto-deleted)|
|/usr	|User-related programs and data|
|/var	|Variable data (like logs, mails)|

## Basic Shell Commands in Linux (With Syntax)
|Command|	Description	|Syntax|
|-------|-------------|------|
|**ls**|	Lists files and folders	|ls [options]|	
|**cd**|	Changes directory	|cd [directory]|
|**mkdir**	|Creates a new folder	|mkdir [folder_name]|
|**rmdir**|	Removes an empty folder	|rmdir [folder_name]|	
|**touch**|	Creates a new empty file	|touch [file_name]|
|**rm**	|Removes files or folders	|rm [file/folder]|
|**cp** |	Copies files/folders	|cp [source] [destination]|	
|**mv**	|Moves or renames files/folders	|mv [source] [destination]|	
|**cat** |Displays contents of a file	|cat [file_name]|	
|**whatis**|	Gives a one-line description of a command	|whatis [command]|
|**whereis**	|Shows location of binary, source, and man page	|whereis [command]|	
|**clear**	|Clears the terminal screen	|clear|	
|**man**	|Shows manual/help for a command	|man [command]|	
|**exit**	|Closes the terminal session		|exit|
|**pwd**	|Shows current directory path	|	pwd|
|---------|-----------------------------|----|

![image](https://github.com/user-attachments/assets/d93c2a88-79e1-4d03-a82b-7914cdcbcd34)
![image](https://github.com/user-attachments/assets/a2aadfc4-a485-4784-bf6b-14e684a767cf)
![image](https://github.com/user-attachments/assets/fb854dc0-5499-4f6f-99e6-b5b872b1af66)


