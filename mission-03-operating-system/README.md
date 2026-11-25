# Mission 3 — Operating system, processes and permissions

## 1. Task / objective

Explore the operating system, running processes, storage, paths and file permissions, and explain core OS responsibilities.

## 2. Work completed

### Task 3.1 — Operating-system observations

| Information explored | What it tells you | Privacy-safe observation |
|---|---|---|
| Operating system / system details | Identifies the operating system and hardware architecture. | macOS 27.2.1 is running on an arm64 architecture. |
| Current account identity | Identifies the account session that is allowed to start processes and access files. | The active account identity was [redacted]. |
| Available and used storage | Shows root-volume capacity and how much space is in use. | The root volume reported 460 GiB capacity, 381 GiB available and approximately 13 GiB used. |
| System activity snapshot | Shows running processes and their process identifiers. | A snapshot contained launchd as PID 1 and background services such as logd and systemstats. |

### Task 3.2 — Processes

A process is a running program or instance of a program, including its current memory and execution state.

- The PID column contains the process identifier assigned to a running process. It distinguishes processes and allows the system to refer to one process.
- Examples: `launchd`, the macOS system-launch process, and `Safari`, a browser process, may appear while they are running.

### Task 3.3 — Paths and permissions

An absolute path starts at the filesystem root and identifies a location completely. One absolute path for this assignment is `/Users/[redacted]/Documents/digital-dectective-8479/mission-02-terminal/terminal-practice/practice.txt`.

A relative path starts from the current working directory. From the project root, `mission-02-terminal/terminal-practice/practice.txt` is a relative path.

Navigation from the project folder to Mission 2 changes the displayed location from the project root to the Mission 2 subfolder. The detailed listing of `practice.txt` showed `-rw-r--r--`, so the owner has:

| Permission | Meaning | Example |
|---|---|---|
| `r` — Read | Allows file contents to be read. | Owner can open `practice.txt`. |
| `w` — Write | Allows file contents to be changed. | Owner can edit `practice.txt`. |
| `x` — Execute | Allows a file to be run as a program or a directory to be traversed. | Not set for this text file. |

### Task 3.4 — Operating-system responsibilities

| OS responsibility | Explanation | Example |
|---|---|---|
| Process management | Creates, schedules and stops processes while sharing processor time. | The OS lets a browser and text editor run together. |
| Memory management | Allocates memory to running programs and recovers memory that is no longer used. | RAM is assigned to VS Code while a document is open. |
| Device management | Uses drivers to communicate with keyboards, displays, disks and other devices. | A key press is delivered to a text editor. |
| File management | Organises files and folders and controls reading and writing. | The OS stores Mission 2 notes in named directories. |
| User interface / shell | Provides a graphical or command-line way to interact with the system. | Finder or Terminal accepts user commands. |
| Security and permissions | Controls identities, access rights and protected resources. | A file can be read or written only where permissions allow it. |

## 3. Commands / tools used

- `sw_vers -productName` and `sw_vers -productVersion` — display macOS details.
- `uname -m` — identifies the system architecture.
- `df -h /` — reports root-volume storage information.
- `ps -axo pid,comm` — lists process IDs and process names.
- `cd`, `pwd` and `ls -l` — navigation, location and permission inspection.
- Activity Monitor / browser — could display application and background processes.

## 4. My understanding

An operating system is the layer that manages hardware and provides common services to applications. Processes run under its supervision; paths identify locations; and permissions control who may read, change or execute a file. Storage details show capacity rather than the contents of files.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- [Mission 2 practice file](../mission-02-terminal/terminal-practice/practice.txt)
- Privacy-safe command observations recorded in this README

## 8. Commit details

- Meaningful commit message: `Document operating system and file management`