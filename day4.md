# Training day 4:- 
## File compression
In Linux, file compression is the process of reducing the size of a file or a set of files using various algorithms to encode data more efficiently, thus saving storage space and optimizing data transfer. It's a fundamental technique for managing files, especially when dealing with large datasets or when transferring files over networks. 
### zipping:-
```
syntax: gzip filename

```

compresses the file filename and replace it with filename.gz
**example:-**

### unzipping:-
```
syntax: gunzip filename.sh.gz

```
![image](https://github.com/user-attachments/assets/c639bb42-f02f-416f-877f-0dce37a47d13)


### want to keep original file too? 
for this, you need to use
`-k zip -k notes.txt`
**how?**
- notes.txt(kept)
- notes.txt.gz(created)
![image](https://github.com/user-attachments/assets/7a0f73ba-eefd-4ac8-b7fd-a3598dc23659)
  
### wildcard(globbing)
### Wild cards:
it matches files without typing full names.
| Wildcard | Meaning    | 
| -------- | --------------------------------------------- |
| `*`      | Matches **zero or more** characters           | 
| `?`      | Matches **exactly one** character             |
| `[abc]`  | Matches **one character** from set            | 

![image](https://github.com/user-attachments/assets/be5bb45d-fdba-4faf-a7ed-a5f00fa90924)


## hardware : PC, hardware troubleshooting :-
### CPU:
The Central Processing Unit (CPU) is like the brain of a computer. It’s the part that does most of the thinking, calculating, and decision-making to make your computer work. Whether you’re playing a game, typing a school assignment, or watching a video, the CPU is busy handling all the instructions to get the job done.
![image](https://github.com/user-attachments/assets/aff29abb-5f14-42e3-b333-5418e5b662ff)

**components of CPU**

**1.Motherboard (printed circle board)**
![image](https://github.com/user-attachments/assets/786bac4e-ccee-4a7f-9a66-395e859db98e)

A motherboard is the central circuit board in a computer that connects all the other components. It acts as the nervous system, allowing communication between the CPU, RAM, storage devices, and expansion cards. Key components include the CPU socket, RAM slots, expansion slots, chipset, BIOS/UEFI, and various ports for peripherals. 
Key Components and their Functions:
- CPU Socket:
This is where the processor (CPU) is installed. It provides the physical connection and electrical interface for the CPU. 
- RAM Slots:
These slots allow for the installation of Random Access Memory (RAM), which temporarily stores data the CPU is actively using. 
- Expansion Slots (PCIe, PCI):
These slots allow for the installation of expansion cards like graphics cards, sound cards, or network cards, increasing the functionality of the computer. 
- Chipset:
The chipset acts as a bridge, connecting the CPU, memory, and other peripherals. It manages data flow and communication between these components.
Types of Chipsets:
Historically, chipsets were divided into two main parts: the Northbridge and Southbridge. 
Northbridge: Managed high-speed communication between the CPU, RAM, and graphics card. 
Southbridge: Managed slower peripherals like USB ports, hard drives, and audio interfaces. 
- BIOS/UEFI:
The Basic Input/Output System (BIOS) or Unified Extensible Firmware Interface (UEFI) is firmware that initializes and tests hardware during startup and provides runtime services to the operating system. 
- Storage Connectors (SATA):
These connectors allow for the connection of storage devices like hard drives (HDD) and solid-state drives (SSD). 
- Power Connectors:
These connectors deliver power to the motherboard and its components from the power supply. 
- Input/Output Ports (USB, Audio, Ethernet):
These ports on the back panel of the computer allow for the connection of peripherals like keyboards, mice, monitors, and external storage devices. 
- fan:
It plays a crucial role in maintaining the optimal temperature of the central processing unit(CPU) within a computer.
-diodes:
They control the direction of electrical current.
- Modem(LAN card):
It is used to convert digital data(0 and 1) from your computer into analog signals that can travel over communication lines.
- transistors:
They act as tiny electronic switches that control the flow of electrical current. They are the fundamental building blocks of the CPU, enabling it to perform calculations and process information by switching between "on" and "off" states. These transistors are combined to create logic gates, which form more complex circuits, ultimately allowing the CPU to execute instructions and perform tasks. 
- CMOS :
CMOS refers to Complementary Metal-Oxide-Semiconductor, a type of technology used in the chip's design. It's not a physical component within the CPU itself, but rather a technology used to manufacture the CPU and other electronic components. CMOS technology allows for low power consumption and high-speed performance, making it ideal for microprocessors like those found in CPUs

- Other Connectors:
These include connectors for front panel buttons and LEDs, as well as headers for additional USB ports and other internal components. 

**2. Hard Disk Drive (HDD):**
- Stores data,software, and the operating system.
- Located under the optical drive in the cabinet.

**3.optical drive(CD/DVD Drive):**

* Used to read/write **CDs and DVDs**

*How to locate components of a CPU?*

- Look for the power supply with fan (usually at the back top or bottom of the cabinet).
- In front of it is the optical drive.
- On it's side is the Motherboard.
- Below the optical drive is the hard disk drive.
###  What Happens When You Power On Your PC (Hardware Level)

1. **Power supply starts**  
   - Sends power to all components.

2. **CPU wakes up**  
   - Looks for instructions from BIOS/UEFI.

3. **BIOS/UEFI runs**  
   - Performs POST (Power-On Self-Test) to check hardware.

4. **Boot device is found**  
   - Searches for a bootable device like SSD/HDD.

5. **Bootloader is loaded**  
   - Loads a small program into RAM.

6. **Operating system starts loading**  
   - The OS kernel takes control and the system starts.
### Difference between RAM and Cache memory:

| Feature        | **RAM (Random Access Memory)**            | **Cache Memory**                          |
| -------------- | ----------------------------------------- | ----------------------------------------- |
| **Purpose**    | It holds programs and data that are currently executed by the CPU. | It holds frequently used data by the CPU.  |
| **Speed**      | Slower than cache                         | Much faster than RAM                      |
| **Size**       | Larger (in GBs, e.g., 8GB, 16GB)          | Smaller than RAM  |

**Why do we need Cache memory?**
- It helps the **CPU work faster and more efficiently** by reducing the time it takes to access data.
  * Cache memory is **much faster** than RAM.
  * It stores **frequently used instructions and data**, so the CPU doesn’t have to wait for slower RAM.
  * Without cache, the Processor would **waste cycles**.<br>
So it is used to remove mismatch between RAM and Processor speed.

### Difference between RAM and Hard Disk:

| Feature              | RAM (Random Access Memory)           | Hard Disk                            |
| -------------------- | ----------------------------------------------- | ---------------------------------------------- |
| **Purpose**          | Temporary memory for currently running programs | Permanent storage for files, software, and OS  |
| **Storage Type**   | Temporary (loses data when off)                   | Permanent (keeps data when off)|
| **Speed**            | Much faster                                     | Slower compared to RAM                         |
| **Storage Capacity** | Smaller                   | Larger                  |
| **Access Method**    | Direct access by CPU                            | Slower access through file system              |
| **Cost**      |  Expensive                                  | Cheaper                                        |
| **Function**         | Helps run active programs and processes         | Stores data, files, OS, and installed programs |



