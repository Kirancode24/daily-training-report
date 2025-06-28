# Training day 3

### Dual Boot
Dual booting allows a computer to run two different operating systems, enabling users to choose which one to boot into upon startup.

### ISO file
In Linux, an ISO file is a single file containing a complete copy of the data from a CD, DVD, or other optical media, formatted as an ISO 9660 file system. 

### Bare metal installation
It refers to setting up an operating system directly on a physical server's hardware, without any intervening virtualization layer like a hypervisor.

### VMware and Virtual box
VMware is a commercial product known for its enterprise-grade features, performance, and comprehensive support, while VirtualBox is an open-source, free alternative, generally favored for personal use, testing, and development. 

### Partitioning schemes
1. Dividing a hard disk into separate sections.

2.Each section (partition) acts like an independent disk.

3.Helps organize data and install multiple OS.

### Types
- MBR (Master Boot Record):

1. Max 4 primary partitions.

2. Supports up to 2 TB.

3. Older, used with BIOS.

4. less flexible

- GPT (GUID Partition Table):

1. Supports 128+ partitions.

2.Works with disks >2 TB.

3.Newer, used with UEFI.

4.more flexible

### Permissions & Shell programming:
### File and directory permissions:

**chmod (Change mode)**: It is used to change the access permissions of files and directories.

### Some different chmod permission notations are:
**chmod +x test.sh**: Gives permission to run the script.
**chmod 444 test.sh**: Changes file to read-only

### result


**chmod 644 test.sh**: Changes file such that only owner can edit it. For others it remain read-only.



### result


### Redirection:
In Linux, whenever an individual runs a command, it can take input, give output, or do both. Redirection helps us redirect these input and output functionalities to the files or folders we want, and we can use special commands or characters to do so.

### Types of Redirection:

### Overwrite Redirection (For stdout):
Overwrite redirection is useful when you want to store/save the output of a command to a file and replace all the existing content of that file. for example, if you run a command that gives a report, and you want to save the report to the existing file of the previous report you can use overwrite redirection to do this. 

**">" standard output**
![image](https://github.com/user-attachments/assets/490f02ed-2988-410a-b1ec-3ec168ad0d0a)


### Append Redirection (For stdout): 
With the help of this Redirection, you can append the output to the file without compromising the existing data of the file.
![image](https://github.com/user-attachments/assets/ff0e161f-a6e9-4124-ba7a-9a5b59daf306)



### Overwrite Redirection (For stdin):
Redirects the standard input of a command to a file.
**"<" standard input**

### sorting with help of Redirection:
![image](https://github.com/user-attachments/assets/8b74cef9-c076-43c6-ab56-a64962de290d)

### Pipe '|':
A pipe is a form of redirection (transfer of standard output to some other destination) that is used in Linux and other Unix-like operating systems to send the output of one command/program/process to another command/program/process for further processing.You can make it do so by using the pipe character '|'. 
**Pipe for filtration:**
![image](https://github.com/user-attachments/assets/8808cfb7-0107-4e26-b945-9fe2e2d39847)

**for finding multiple files:**
to find number of files/directory consisting p

![image](https://github.com/user-attachments/assets/0d25e490-2d83-468c-a37c-4b7c3ec27ab2)




### Shell programming:
1.use of variables:
![image](https://github.com/user-attachments/assets/a721b6bd-5557-46b5-880f-a219fa7ddbbf)

output:
![image](https://github.com/user-attachments/assets/93160168-e7de-48fa-bd31-146bf32f09a7)

2.multiply table:
![image](https://github.com/user-attachments/assets/9c73142a-c9ba-43ec-aa95-4cc07a2ec1f5)

output:
![image](https://github.com/user-attachments/assets/fe4da1e0-537d-430a-aa24-09fb4170635f)

3.comparison of two numbers:
![image](https://github.com/user-attachments/assets/d8bfa897-1225-4770-8c2f-3805bcacad69)

output:
![image](https://github.com/user-attachments/assets/1d3a9c57-3120-45e5-a0b4-74abb0c26f91)
