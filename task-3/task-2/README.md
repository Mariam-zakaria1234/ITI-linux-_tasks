# 🐧 Linux CLI Basics - Practical Workspace

## 🎯 Overview
This document contains the execution log and notes for my first hands-on Linux lab. The primary focus of this exercise is mastering fundamental Bash command-line interface (CLI) operations, managing directory trees, inspecting text files, and navigating the standard Linux file system structure.

---

## 🧭 Command Cheat Sheet & Lab Operations

### 📂 Navigation & Directory Control
* `pwd` — Prints the current working directory path.
* `cd <dir>` — Changes directory to the target path.
* `ls -la` — Lists all contents (including hidden files starting with `.`) with full attributes.

### 📝 File Creation & Manipulation
* `mkdir -p <path>` — Creates new folders (including parent directories if needed).
* `touch <file>` — Instantiates new empty files.
* `cp <src> <dest>` — Copies files or folders to a specified location.
* `mv <src> <dest>` — Moves or renames resources within the system.
* `rm` / `rmdir` — Deletes specified files or empty directories.

### 🔍 Viewing & Searching
* `cat` — Prints the full file payload to the terminal.
* `head` / `tail` — Displays the beginning or end of text streams.
* `find` — Locates files based on filenames or conditions.
* `tree` — Generates a visual tree diagram of the current directory hierarchy.

---

## 🧱 The Linux Filesystem Architecture (FHS)

Below is a breakdown of the key system directories explored during the session:

* **`/` (Root):** Top-level directory of the system hierarchy.
* **`/home`:** Contains individual user workspace profiles.
* **`/etc`:** Stores system-wide configurations and service files.
* **`/usr`:** Holds user binaries, libraries, and secondary applications.
* **`/var`:** Stores dynamic data such as system logs, caches, and spools.
* **`/tmp`:** Temporary storage cleared upon reboot.
* **`/dev`:** Hardware interface files representing attached devices.
* **`/proc`:** Virtual filesystem providing real-time kernel & process information.
* **`/boot`:** Contains files necessary for booting the operating system.

---

## 💻 Hands-on Command Execution

```bash
# Check initial location
pwd

# Build project directory tree
mkdir -p MyWorkspace/LinuxBasics
cd MyWorkspace/LinuxBasics

# Create sub-folders and test file
mkdir -p Docs Research Sandbox
touch notes.txt

# Inspect structure
ls -F
tree
