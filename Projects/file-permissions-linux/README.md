# Linux File Permissions

## Overview

This project demonstrates how Linux file permissions were reviewed and modified to improve system security. The objective was to ensure that files and directories within the `projects` directory followed the organization's access control policy by granting permissions only to authorized users.

---

## Project Objective

The research team identified that several files and directories had permissions that did not comply with the organization's security requirements. The task involved auditing the existing permissions and updating them using Linux commands to enforce the Principle of Least Privilege.

---

## Skills Demonstrated

* Linux Administration
* Linux File Permissions
* Access Control
* Principle of Least Privilege (PoLP)
* Cybersecurity Fundamentals
* Command-Line Interface (CLI)
* Security Hardening

---

## Tools Used

* Linux Terminal
* `ls`
* `chmod`

---

## Tasks Performed

* Inspected file and directory permissions using `ls -la`
* Interpreted Linux permission strings
* Removed unauthorized write permissions from project files
* Updated permissions for a hidden archived file
* Restricted directory access to authorized users only
* Verified all permission changes after implementation

---

## Linux Commands Used

```bash
# View file and directory permissions
ls -la

# Remove write permission for others
chmod o-w project_k.txt

# Remove write permission from the file owner
chmod u-w .project_x.txt

# Remove write permission from the group and grant read permission
chmod g-w,g+r .project_x.txt

# Remove execute permission from the group
chmod g-x drafts
```

---

## Security Improvements

| Item             | Action Taken                                                                         |
| ---------------- | ------------------------------------------------------------------------------------ |
| `project_k.txt`  | Removed write permission from other users                                            |
| `.project_x.txt` | Removed write permission from the owner and group; ensured read access for the group |
| `drafts/`        | Removed execute permission from the group so only the owner retained access          |

---

## Key Concepts Applied

* File Ownership
* User, Group, and Other Permissions
* Read (`r`), Write (`w`), and Execute (`x`) Permissions
* Hidden Files
* Directory Permissions
* Principle of Least Privilege

---

## Learning Outcomes

Through this project, I gained practical experience with:

* Managing Linux file permissions
* Securing files using the `chmod` command
* Auditing file system access
* Applying least-privilege access controls
* Strengthening Linux system security

---

## Repository Structure

```
file-permissions-linux/
├── README.md
├── File permissions in Linux.pdf
└── Before file permissions.pdf
```

---

## Author

**Pankaj Swami**

Aspiring Cybersecurity Professional | Linux | Network Security | SOC Analyst

---

*This project was completed as part of my cybersecurity learning portfolio to demonstrate practical Linux security and access control skills.*
