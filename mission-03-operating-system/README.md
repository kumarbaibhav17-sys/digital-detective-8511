# Mission 3 — Understand the operating system

## 1. Task / objective
Explore the operating system, running processes, storage, paths and file permissions, and describe the responsibilities of an OS.

## 2. Work completed

### Task 3.1: Explore my operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
|---|---|---|
| Operating system / system details | Which OS and version the computer is running | i am currently on macOS, version [27.2]. Computer name: [Mac] |
| Current account identity | Which user account is currently active | The active account is [####] |
| Available and used storage | How much disk space is used and how much is free | The main disk has about [460 GB] in total and [171 GB] free |
| System activity snapshot | A quick look at CPU use, memory use and running tasks | It showed about [706] processes and CPU usage of about [19.50%] |

### Task 3.2: Understand processes
I ran `ps aux | head -n 10` and looked at the PID column.

- **What is a process?** A process is a program that is currently running on the computer.
- **What does the PID column represent?** PID is the process identifier, a unique number the operating system gives to each running process so it can track and manage it.
- **Two examples of processes on my computer:** [process 1,Google Chrome] and [process 2,VS-CODE].

### Task 3.3: Paths and permissions
I moved from the assignment folder into `mission-03-operating-system` and back with `cd`, and checked the location with `pwd`. The path shown got longer when I went into the subfolder and shorter when I came back.

- **Absolute path:** the full path starting from the top of the file system. Example: /Users/[####]/digital-detective-8511
- **Relative path:** a path that starts from the folder I am currently in. Example: mission-03-operating-system/README.md

I ran `ls -l README.md` and looked at the permission letters. The owner's permissions were `[e.g. rw-]`, which means the owner can read and write the file but cannot execute it. I did not change any permissions.

### Task 3.4: Operating system responsibilities

| OS responsibility | Your explanation | Example |
|---|---|---|
| Process management | The OS decides which programs run, when they run and for how long, so many programs can work together | Using Chrome and VS Code at the same time |
| Memory management | The OS gives each running program the RAM it needs and takes it back when the program closes | Opening many browser tabs uses more RAM, and closing them frees it |
| Device management | The OS controls hardware such as the keyboard, screen and printer through drivers | Sending a document to a printer |
| File management | The OS organises how files and folders are stored, named, found and opened on the disk | Saving a file in a folder and opening it later |
| User interface / shell | The OS gives the user a way to communicate with it, through windows and icons or typed commands | Using Finder icons or typing commands in the Terminal |
| Security and permissions | The OS controls who can access which files and what they can do with them | Only the file's owner being able to edit it |


