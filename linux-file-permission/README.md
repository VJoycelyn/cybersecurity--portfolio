# Linux File Permissions Review

## 📁 Folder: `incident-response/linux-file-permissions/`

This project showcases my ability to use Linux commands to manage file and directory permissions, an essential task during cybersecurity incident response to limit unauthorized access and restore secure configurations.

---

## 🔍 Project Description
As part of the incident response process, I conducted a permissions audit on the `/home/researcher2/projects` directory. I used standard Linux commands to:
- Identify misconfigured permissions
- Interpret permission strings
- Correct insecure file and directory access

These tasks are key to preventing data leakage and maintaining confidentiality, integrity, and availability during and after an incident.

---

## 🛠️ Commands Used

### 1. **List All File Permissions**
```bash
ls -la /home/researcher2/projects
```
Used to view all files, including hidden ones, and their permissions in long format.

### 2. **Fix Overly Permissive File (Others write access)**
```bash
chmod o-w project_k.txt
```
Removes write permissions from others.

### 3. **Secure Hidden Archived File**
```bash
chmod 440 .project_x.txt
```
Grants read-only access to the user and group.

### 4. **Restrict Directory to Owner Only**
```bash
chmod 700 drafts
```
Ensures only `researcher2` can access the `drafts` directory.

---

## 🧠 What I Learned
- How to interpret and explain 10-character permission strings (e.g., `-rw-rw-r--`)
- Proper syntax and use of `chmod` for both files and directories
- Importance of access control during incident investigation and remediation

---

## 🖼️ Screenshots Folder (Optional)
Place screenshots of terminal output showing before/after permissions:
```
screenshots/
├── ls-la_output.png
├── chmod_project_k.png
├── chmod_hidden_file.png
└── chmod_directory.png
```

---

## ✅ Summary
This exercise demonstrates my ability to take action on insecure file permissions using Linux. These foundational skills help reduce risk exposure during incident response by hardening access controls across the file system.

