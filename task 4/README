# 🛠️ Lab Log: Custom Bash Shell Functions (Assignment 4)

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
