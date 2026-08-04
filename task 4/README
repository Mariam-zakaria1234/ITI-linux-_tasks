## 🛠️ Lab Log: Custom Bash Shell Functions (Assignment 4)

## 📌 Overview
This assignment extends the functionality of the Bash terminal by defining a set of reusable shell functions in `~/.bashrc`. These helper functions streamline daily command-line workflows, including filesystem navigation, safe deletion, directory generation, and file searching.

---

## 🎯 Key Objectives
- Design custom alias-like utility functions in Bash.
- Simplify complex or repetitive CLI commands into short, intuitive helpers.
- Configure persistent commands across all user terminal sessions.

---

## 🛠️ Function Implementations & Code Snippets

The following shell functions were appended to `/home/mariam/.bashrc`:

```bash
# 1. Directory Listing
print_content() {
    ls -la
}

# 2. Directory Navigation
go_to() {
    cd "$1"
}

# 3. Highlighted Keyword Search
search() {
    grep --color=always -n "$1" "$2"
}

# 4. Numbered File Inspection
show_file() {
    nl "$1"
}

# 5. Interactive Safe Removal
remove() {
    rm -i "$1"
}

# 6. Nested Directory Creation
make_dir() {
    mkdir -p "$1"
}

# 7. Blank File Creation
create_file() {
    touch "$1"
}
🔄 Activation & Reload
To apply these new functions instantly to user mariam's active terminal session:

Bash
source ~/.bashrc
💻 Custom Commands Reference
Command Syntax	Functionality
print_content	Lists all files including hidden dotfiles in detailed format
go_to <path>	Navigates directly to the specified path
search <term> <file>	Searches for text within a file, displaying line numbers and highlighted matches
show_file <file>	Prints file contents with sequential line numbering
remove <file>	Requests user confirmation (y/n) prior to deleting
make_dir <path>	Generates a full directory tree including missing parent paths
create_file <file>	Instantiates a new empty file
🧠 Why modify ~/.bashrc?
User-defined functions created during an active session disappear when the terminal closes. By saving these function definitions inside /home/mariam/.bashrc, Bash loads them automatically into memory every time mariam opens a new interactive shell.

📸 File Snapshot
Below is the verified block appended to the user profile config:

Plaintext
mariam@ubuntu:~$ tail -n 25 ~/.bashrc

# --- Custom Shell Utilities ---
print_content() { ls -la; }
go_to() { cd "$1"; }
search() { grep --color=always -n "$1" "$2"; }
show_file() { nl "$1"; }
remove() { rm -i "$1"; }
make_dir() { mkdir -p "$1"; }
create_file() { touch "$1"; }
📁 Repository Structure
Plaintext
Assignment4/
└── README.md
👤 Student Profile
Student: Mariam

Track: ITI Embedded Systems

Status: ✅ Completed
