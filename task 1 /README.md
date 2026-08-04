.# 🐧 Linux CLI Basics - Lab Report

## 📖 Overview
A foundational hands-on lab focused on mastering the core commands of the Linux terminal using the Bash shell. This module covers essential file system navigation, directory tree management, file inspection tools, and an overview of the Linux Filesystem Hierarchy Standard (FHS).

---

## 🎯 Lab Objectives
- Install and configure the Ubuntu Linux environment.
- Master navigation using both absolute and relative file paths.
- Explore and understand key system directories in the Linux hierarchy.
- Perform core file operations (create, copy, move, rename, and delete).
- Inspect file contents using built-in command-line utilities.

---

## 🛠️ Commands Practiced

| Command | Description |
| :--- | :--- |
| `pwd` | Displays the absolute path of the current working directory |
| `ls` / `ls -la` | Lists directory contents, including hidden dotfiles with metadata |
| `cd` | Changes the current working directory path |
| `mkdir` | Creates new directories or nested directory trees (`-p`) |
| `touch` | Instantiates empty files or updates file timestamps |
| `cat` | Outputs full text file contents directly to stdout |
| `head` / `tail` | Previews the beginning or end of text files |
| `cp` | Copies files and folders to a target location |
| `mv` | Moves or renames files and directories |
| `rm` / `rmdir` | Removes specified files or empty directories |
| `find` | Searches the file system based on filename or attributes |
| `tree` | Renders a visual structural tree of folders and files |

---

## 📦 Linux Filesystem Hierarchy (FHS)

Below are the core system directories examined during the session:

| Directory | Purpose |
| :--- | :--- |
| `/` | The top-level root directory of the whole system |
| `/home` | User personal directories and workspace environments |
| `/etc` | Global system configurations and boot script settings |
| `/usr` | System applications, binaries, and shared libraries |
| `/var` | Variable dynamic data files (logs, spools, and caches) |
| `/tmp` | Storage for temporary session files cleared on system restart |
| `/dev` | Virtual files representing attached physical hardware devices |
| `/proc` | Pseudo-filesystem containing real-time kernel & process states |
| `/boot` | Critical bootloader configs and Linux kernel images |

---

## 📷 Example Terminal Session

```bash
mariam@ubuntu:~$ pwd
/home/mariam

mariam@ubuntu:~$ mkdir LinuxPractice
mariam@ubuntu:~$ cd LinuxPractice
mariam@ubuntu:~/LinuxPractice$ mkdir Documents Projects Notes
mariam@ubuntu:~/LinuxPractice$ touch lesson.txt
mariam@ubuntu:~/LinuxPractice$ ls
Documents  Notes  Projects  lesson.txt

mariam@ubuntu:~/LinuxPractice$ cat lesson.txt
Welcome to Linux!
