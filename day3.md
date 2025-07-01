
# Training day 3

### ISO file
In Linux, an ISO file is a single file containing a complete copy of the data from a CD, DVD, or other optical media, formatted as an ISO 9660 file system. 

### Dual Boot
Dual booting allows a computer to run two different operating systems, enabling users to choose which one to boot into upon startup.

### VMware and Virtual box
VMware is a commercial product known for its enterprise-grade features, performance, and comprehensive support, while VirtualBox is an open-source, free alternative, generally favored for personal use, testing, and development. 

### Bare metal installation
It refers to setting up an operating system directly on a physical server's hardware, without any intervening virtualization layer like a hypervisor.

### Partitioning schemes
1. Dividing a hard disk into separate sections.

2. Each section (partition) acts like an independent disk.

3. Helps organize data and install multiple OS.

**Types**
- MBR (Master Boot Record):

1. Max 4 primary partitions.

2. Supports up to 2 TB.

3. Older, used with BIOS.

4. less flexible

- GPT (GUID Partition Table):

 1. Supports 128+ partitions.

 2. Works with disks >2 TB.

 3. Newer, used with UEFI.

 4. more flexible

### Permissions & Shell programming:
### File and directory permissions:

**chmod (Change mode)**: It is used to change the access permissions of files and directories For the owner, group,and others.
**syntax** :
```bash
chmod [permissions] [file_name]
```
**For example:** chmod + x filename.sh

##  `chmod +x filename.sh`

The command `chmod +x filename.sh` is used to **add execute permission** to a file (usually a script like `.sh`), so it can be **run as a program**.

---

###  Syntax Breakdown

| Component     | Description                                                  |
| ------------- | ------------------------------------------------------------ |
| `chmod`       | Stands for **Change Mode** – used to change file permissions |
| `+x`          | Adds **execute** permission                                  |
| `filename.sh` | The name of the shell script file                            |

---


###  Purpose

This command makes a file **executable** by the **user, group, and others (by default)**.
You can then run the script directly using:

```bash
./filename.sh
```

Without execute permission, you'll see:

```
bash: ./filename.sh: Permission denied

```

To give execute permission **only to the file owner**, use:

```bash
chmod u+x filename.sh
```
This is a safer option when sharing code in teams or on public systems.

---


####  **Octal Permission Codes**:

| Number | Symbol | Meaning              |
| ------ | ------ | -------------------- |
| 7      | rwx    | Read, Write, Execute |
| 6      | rw-    | Read, Write          |
| 5      | r-x    | Read, Execute        |
| 4      | r--    | Read only            |
| 0      | ---    | No permissions       |

---
### example:
**chmod +x test.sh**: Gives permission to run the script.
- chmod 444 test.sh: Changes file to read-only
![image](https://github.com/user-attachments/assets/75fe6c43-31e1-4dc7-b20e-24970039ffbf)
r-- r-- r--
### result
![image](https://github.com/user-attachments/assets/b1102f24-e2b5-49e7-ba42-4624b40367ad)


- chmod 644 test.sh: Changes file such that only owner can edit it. For others it remain read-only.
![image](https://github.com/user-attachments/assets/18c8aa08-6611-430a-84b3-deeb307c9488)

rw- r-- r--

### result
![image](https://github.com/user-attachments/assets/60bad556-a1a9-4ec2-8eb9-c2c689ae4c95)

### chown :

**How to Use `chown`:**
 1. Check current ownership (optional).
 2. Run the `chown` command.  Use `sudo` if you're not the current owner.
**used for**
**Changing owner only:**<br>

**Changing group only:**<br>


**Changing both group and owner permissions:** <br>







### Redirection:
In Linux, whenever an individual runs a command, it can take input, give output, or do both. Redirection helps us redirect these input and output functionalities to the files or folders we want, and we can use special commands or characters to do so.

### Types of Redirection:

- Overwrite Redirection (For stdout):
Overwrite redirection is useful when you want to store/save the output of a command to a file and replace all the existing content of that file. for example, if you run a command that gives a report, and you want to save the report to the existing file of the previous report you can use overwrite redirection to do this. 

**">" standard output**


- Append Redirection (For stdout): 
With the help of this Redirection, you can append the output to the file without compromising the existing data of the file.
![image](https://github.com/user-attachments/assets/6c03f723-615b-48c4-b843-2df66bc906de)
![image](https://github.com/user-attachments/assets/1543d4f1-6a42-4fae-aa2d-93e603271aae)



- Overwrite Redirection (For stdin):
Redirects the standard input of a command to a file.
**"<" standard input**


### sorting with help of Redirection:
![image](https://github.com/user-attachments/assets/4b4384aa-1975-4945-ae77-be411d2442f3)


### Pipe '|':
A pipe is a form of redirection (transfer of standard output to some other destination) that is used in Linux and other Unix-like operating systems to send the output of one command/program/process to another command/program/process for further processing.You can make it do so by using the pipe character '|'. 
**Pipe for filtration:**
![image](https://github.com/user-attachments/assets/3f2db4f6-0432-420b-b3f3-9e99242f2d33)


**for finding multiple files:**
to find number of files/directory consisting p
![image](https://github.com/user-attachments/assets/17b7abd9-9516-49fa-883c-b8e680021439)




### Shell programming:
1.use of variables:
![image](https://github.com/user-attachments/assets/c6ed06be-0a47-4d65-8267-33436d9f8604)


output:
![image](https://github.com/user-attachments/assets/aef78e87-5464-458a-98f6-c4489b6f09bc)



2.multiply table:
![image](https://github.com/user-attachments/assets/9495dccb-f5d0-468c-a412-5731a1f0c447)



output:
![image](https://github.com/user-attachments/assets/a44d6734-c8d6-4d62-b4f0-ba1e658acbd3)


3.comparison of two numbers:
![image](https://github.com/user-attachments/assets/3beddb41-6150-4e46-904b-66839f4e786f)



output:
![image](https://github.com/user-attachments/assets/4d69105e-01e0-4fba-8543-c10495a7a6eb)

