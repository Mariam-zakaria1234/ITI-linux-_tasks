# 📋 Lab Log: Employee Registration Bash Script (Assignment 5)

## 📌 Overview
This assignment introduces foundational Bash scripting concepts by building an interactive command-line **Employee Registration System**. The script accepts live input from the terminal user, stores data in local variables, and prints a structured summary report.

---

## 🎯 Key Objectives
- Write and execute a standalone executable Bash script (`.sh`).
- Capture interactive user inputs via the terminal prompt (`read`).
- Store and reference values using local shell variables.
- Output formatted text reports back to stdout.
- Manage script execution permissions using `chmod`.

---

## 🛠️ Script Source Code (`emp.sh`)

Below is the implementation stored inside `emp.sh`:

```bash
#!/bin/bash

echo "====================================="
echo "    Employee Registration System"
echo "====================================="
echo ""

read -p "Enter Employee Name: " name
read -p "Enter Employee Age: " age
read -p "Enter Department: " department
read -p "Enter Salary: " salary

echo ""
echo "====================================="
echo "      Employee Information"
echo "====================================="
echo "Name       : $name"
echo "Age        : $age"
echo "Department : $department"
echo "Salary     : $salary"
echo "====================================="
🚀 Script Execution Setup
To grant execute permissions and run the script:

Bash
# 1. Add execution rights
chmod +x emp.sh

# 2. Run the script directly
./emp.sh
💻 Sample Terminal Session
Plaintext
mariam@ubuntu:~/Assignment5$ ./emp.sh
=====================================
    Employee Registration System
=====================================

Enter Employee Name: Mariam
Enter Employee Age: 22
Enter Department: Embedded Systems
Enter Salary: 10000

=====================================
      Employee Information
=====================================
Name       : Mariam
Age        : 22
Department : Embedded Systems
Salary     : 10000
=====================================
📚 Core Bash Concepts Applied
Concept	Usage	Description
Shebang	#!/bin/bash	Specifies Bash as the script interpreter
Input Capture	read -p "prompt" var	Prompts user and stores terminal input in a variable
Variables	$name, $age, etc.	Holds runtime employee parameters
Output Styling	echo	Prints headers and organized output blocks
Permissions	chmod +x emp.sh	Converts the text file into an executable program
📁 Repository Structure
Plaintext
Assignment5/
├── emp.sh
└── README.md
👤 Student Profile
Student: Mariam

Track: ITI Embedded Systems

Status: ✅ Completed
