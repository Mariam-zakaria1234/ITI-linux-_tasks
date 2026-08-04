# 🖥️ Lab Log: Customizing Terminal Welcome Screen (Assignment 3)

## 📌 Overview
This lab focuses on configuring the interactive Bash shell environment to output a clean, dynamic system summary banner upon initializing any new terminal session.

---

## 🎯 Key Objectives
- Customize the automatic startup sequence of the Bash shell.
- Create a dynamic greeting script displaying real-time system metrics.
- Configure `~/.bashrc` to ensure automatically executing the banner on every terminal launch.

---

## 🛠️ Script Setup & Implementation

To construct the startup screen, the following shell commands and environment variables were added directly to the bottom of `~/.bashrc`:

```bash
# Clear screen on session startup
clear

echo "=========================================="
echo "      Welcome to ITI Linux Environment"
echo "=========================================="
echo ""
echo "User        : $USER"
echo "Hostname    : $(hostname)"
echo "Date        : $(date)"
echo "Shell       : $SHELL"
echo "Current Dir : $(pwd)"
echo ""
echo "Have a productive day!"
echo "=========================================="
