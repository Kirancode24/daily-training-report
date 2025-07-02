## Training day 5:-
---

##  HDD Types and Components
**HDD (Hard Disk Drive)** is a **non-volatile storage device** that stores and retrieves digital data using **magnetic storage**. It contains spinning disks (platters) and read/write heads.

---

##  Key Features
- Long-term data storage
- Uses magnetic platters and mechanical arms
- Slower than SSDs
- Large storage capacity at low cost

---

##  Types of HDD

| Type                    | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| **PATA (IDE)**          | Older standard, slow, now obsolete                                           |
| **SATA**                | Common in modern desktops/laptops, faster and more reliable than PATA       |
| **SCSI**                | Used in servers, supports multiple devices, high performance                |
| **SSHD (Hybrid Drive)** | Combines SSD speed with HDD capacity                                        |
| **External HDD**        | Portable, connects via USB, used for backups and additional storage         |
| **Enterprise HDD**      | High-performance, for servers/data centers, designed for 24/7 operation     |

---

##  HDD Form Factors

| Form Factor | Usage               |
|-------------|---------------------|
| 3.5 inch    | Desktop computers   |
| 2.5 inch    | Laptops, compact PCs|

---

## Note:
>  **SSD (Solid-State Drive)** is not a type of HDD, but is often compared with HDD due to similar purpose (storage). SSDs have no moving parts and are much faster.

---

---

##  GPU (Graphics Processing Unit)
- **Definition:** Specialized processor for rendering graphics.
- **Function:** Enhances image processing and supports high-performance computing tasks.
- **Problems:** overheating, driver issues,screen tearing,or no display output
---

## PCU (Personal Computer Unit):

1.installing and hard disk preparation:
### Logical and Extended Partitioning:
- **Logical Partition:**
  - Store the OS (Linux, Unix, Windows) on the C drive.
  - Keep important files off the C drive to prevent loss during crashes.

- **Extended Partition:**
  - Use D, E, or other drives for images, notes, and non-critical files.
2. Speed slow (Causes & Fixes):
- Desktop: Files should be on drive. By default files on desktop are stored on C drive. As OS system is installed in C: file, its recomended to not put many folders in Desktop. Move them into drives. 

- Task bar: Keep minimal shortcuts on the taskbar 

- Browser (Bookmarks): Avoid excessive browser bookmarks as they slow down browser start-up.

- Temporary files: These files are created by websites & cookies, and stored/ download in hidden files. Ulitmately because of it the system slows down.  So, after a period of time remove temporary files.

- RAM overuse: Don't open a number of applications or tabs are open at once. As ulitimately we are using the RAM.

- Malware: Regularly scan your system for malwares.

- Fragmentation: 
    There shouldn’t be dely to access files. 
    To make system efficient in working and get work done in optimal way, defragmentation is done.<br>
    * Go to `Start → Defragment and Optimize Drives`
    * Schedule defragmentation for automatic optimization.
---

##  Speed Optimization

### Steps to Speed Up Your System:
```bash
# 1. Remove Temporary Files

# 2. Disk Cleanup


# 3. Disable Startup Programs


# 4. Defragmentation (Windows Command)

```

- Avoid cluttering the desktop.
- Use minimal bookmarks in browsers.
- Perform regular malware scans.

---

## 5. Printer Issues

### Troubleshooting Steps:
```bash
# Restart the Print Spooler Service


# Check Print Queue


# Reinstall Printer Drivers

```

- If a page gets stuck, cancel and reprint.
- Use the queue for large print jobs.
- Check and replace ink or toner regularly.
## . BSOD (Blue Screen of Death)

### Common Causes:
- **Driver Issues:** Outdated or corrupt drivers can cause BSOD.
- **Hardware Problems:** Faulty RAM or hard drives may trigger BSOD.
- **Software Conflicts:** Incompatible software can lead to system crashes.

### Troubleshooting Steps:
```bash
# 1. Check for Updates
# Ensure Windows and drivers are up to date
wuauclt /detectnow

# 2. Scan for Corrupted Files
sfc /scannow

# 3. Analyze Crash Dumps
# Install WinDbg to analyze dump files
windbg -y SymbolPath -z DumpFilePath

# 4. Test RAM
# Use Windows Memory Diagnostic
echo "Testing RAM" && mdsched

# 5. Check Hard Drive Health
chkdsk /f /r
```

- Record the error code displayed on the BSOD for further troubleshooting.
- Boot into Safe Mode to isolate the issue.
- Uninstall recently added hardware or software if issues persist.

![image](https://github.com/user-attachments/assets/21a5dd90-0d3a-4a6f-9a55-e49bd74d9c0b)
##  BIOS/UEFI Settings and POST Errors

### BIOS/UEFI Settings:
- **Accessing BIOS/UEFI:**
  - Restart the computer and press the appropriate key (usually `F2`, `Del`, or `Esc`) during startup.
- **Common Settings:**
  - Boot Order: Set the priority for bootable devices.
  - Hardware Monitoring: Check system temperatures and fan speeds.
  - Enable/Disable Devices: Turn onboard devices (e.g., LAN, audio) on or off.

### Troubleshooting BIOS/UEFI Issues:
```bash
# Reset BIOS to Default Settings
# Access BIOS and select "Load Defaults" or "Reset to Factory Settings."

# Update BIOS Firmware
# Download the latest firmware from the manufacturer’s website and follow update instructions.

# Clear CMOS
# Power off the system, remove the CMOS battery, and reinsert it after a few minutes.
```

### POST Errors (Power-On Self-Test):
- **Definition:** Diagnostic process performed by the BIOS/UEFI during startup.
- **Common POST Error Codes:**
  - 1 beep: Everything is fine.
  - 2 short beeps: General error, check hardware.
  - Continuous beeping: RAM issue.
  - No beep: Power supply or motherboard problem.

- **Steps to Resolve POST Errors:**
  - Check and reseat RAM modules.
  - Ensure all cables and components are properly connected.
  - Replace faulty hardware if necessary.
