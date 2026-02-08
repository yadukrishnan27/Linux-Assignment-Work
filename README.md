# 1. Create the assignment directory
mkdir -p Yadu_Linux_Assignment
cd Yadu_Linux_Assignment

# 2. Create the Date & Time Script
cat <<EOF > details_date_time.sh
#!/bin/bash
# Script to display student details and system time
clear
echo "=========================================="
echo "       LINUX ASSIGNMENT SUBMISSION        "
echo "=========================================="
echo "STUDENT NAME : Yadu Krishnan.S"
echo "ROLL NUMBER  : 64"
echo "CLASS        : EV4"
echo "------------------------------------------"
echo "EXECUTION DATE & TIME:"
date
echo "=========================================="
EOF

# 3. Create the Inference Document (Observation Report)
cat <<EOF > linux_commands_inference.md
# Command Inference Log - Yadu Krishnan.S

| Command | Result / Inference |
| :--- | :--- |
| \`pwd\` | Confirmed the current working directory path. |
| \`ls -l\` | Viewed file details including permissions and size. |
| \`mkdir\` | Successfully created a new directory structure. |
| \`touch\` | Created an empty file for testing purposes. |
| \`chmod\` | Modified file permissions to allow script execution. |
| \`whoami\` | Verified the current logged-in user identity. |
| \`date\` | Fetched the current system timestamp and calendar. |

**Observation:** Each command provides specific feedback in the terminal, allowing for precise control over the Linux environment.
EOF

# 4. Create the professional README.md
cat <<EOF > README.md
# Linux System Administration - Lab Submission

This repository serves as a formal submission for my **Linux Assignment**. It showcases my understanding of terminal operations, file system hierarchy, and basic automation using shell scripts.

## 📂 Project Documentation

### 1. \`linux_commands_inference.md\`
This document contains a step-by-step log of the commands executed. For every command, I have included a personal inference explaining the system's response.

### 2. \`details_date_time.sh\`
A custom Bash script designed to automate the display of student credentials and real-time system data.

## 🚀 Execution Guide

1. **Set permissions:**
   \`\`\`bash
   chmod 744 details_date_time.sh
   \`\`\`

2. **Execute the script:**
   \`\`\`bash
   ./details_date_time.sh
   \`\`\`

---
### Student Information:
* **Name:** Yadu Krishnan.S
* **Roll No:** 64
* **Class:** EV4
* **Department:** Electronics & VLSI Engineering
EOF

# 5. Final Setup: Make the script executable locally
chmod +x details_date_time.sh

echo "-------------------------------------------------------"
echo "DONE! Your assignment
