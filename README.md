# 🔐 File Access Permission Manager

A command-line based **File Access Permission Manager** developed in C that allows users to create, view, manage, and delete files while controlling file permissions using system-level functions.

This project demonstrates file handling, directory operations, and permission management in C using system calls such as `stat()` and `chmod()`.

## 🚀 Features

- **Create File** – Create a new file in the current directory.
- **View Files** – Display files and directories available in the current working directory.
- **Check Permissions** – View Read, Write, and Execute permissions for Owner, Group, and Others.
- **Grant Permission** – Grant read, write, or execute permission to the file owner.
- **Remove Permission** – Remove read, write, or execute permission from the file owner.
- **Change Permission** – Set permissions manually using octal permission modes such as `644` or `755`.
- **Delete File** – Delete a file with confirmation before removal.

## 🛠️ Technologies Used

- **Programming Language:** C
- **Libraries:** 
  - `stdio.h`
  - `dirent.h`
  - `sys/stat.h`
  - `sys/types.h`
  - `unistd.h`
- **System Calls / Functions:**
  - `stat()`
  - `chmod()`
  - `remove()`
  - `opendir()`
  - `readdir()`
  - `fopen()`

## 📋 Menu Options

| Option | Function |
|---|---|
| 1 | Create File |
| 2 | View Files |
| 3 | Check File Permissions |
| 4 | Grant Permission |
| 5 | Remove Permission |
| 6 | Change Permission |
| 7 | Delete File |
| 8 | Exit |

## 💻 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/File-Access-Permission-Manager.git
```

### 2. Navigate to the Project Folder

```bash
cd File-Access-Permission-Manager
```

### 3. Compile the Program

```bash
gcc main.c -o manager
```

### 4. Run the Program

```bash
./manager
```

## 🔑 Understanding File Permissions

File permissions determine who can read, write, or execute a file.

| Permission | Symbol | Octal Value |
|---|---|---|
| Read | R | 4 |
| Write | W | 2 |
| Execute | X | 1 |

### Example: `755`

- **Owner:** Read, Write, Execute (7)
- **Group:** Read, Execute (5)
- **Others:** Read, Execute (5)

### Example: `644`

- **Owner:** Read, Write (6)
- **Group:** Read (4)
- **Others:** Read (4)

## 📂 Project Structure

```text
File-Access-Permission-Manager/
│
├── main.c
├── manager
├── manager.exe
└── README.md
```

## 🎯 Learning Objectives

- Understand file handling in C.
- Learn directory management using `dirent.h`.
- Understand Linux/Unix file permission concepts.
- Use `stat()` to retrieve file information.
- Use `chmod()` to modify file permissions.
- Implement a menu-driven application.
- Practice system-level programming concepts.

## ⚠️ Platform Compatibility

This program is designed primarily for **Linux/Unix-like operating systems** because it uses POSIX-related functions such as `chmod()`, `stat()`, `opendir()`, and `unistd.h`.

Some functionality may not work directly on Windows without a compatible environment such as MinGW or WSL.

## 👩‍💻 Author

Developed as a C programming and system-level file management project.

---

⭐ If you find this project useful, feel free to explore and improve it!
