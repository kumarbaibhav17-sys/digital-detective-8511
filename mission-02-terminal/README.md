# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Uses the command line to inspect folders, create and manage practice files, and understand flags, pipes and package managers.

## 2. Work completed

### Task 2.1: Basic terminal operations

| Operation / command name | What it does | What I observed |
|---|---|---|
| Current-directory display (`pwd`) | Prints the full path of the folder I'm in | Showed the path ending in digital-detective-8511 |
| Directory listing (`ls`) | Lists files and folders here | Showed the mission folders and README.md |
| Detailed listing (`ls -l`) | Lists with permissions, owner, size and date | Showed one line per item with extra details |
| Change directory (`cd ..`) | Moves to the parent folder | The path shown moved up one level |
| Create directory (`mkdir practice`) | Makes a new folder | A new folder appeared in the listing |
| Create empty file (`touch sample.txt`) | Makes an empty file | sample.txt appeared with size 0 |
| Copy file (`cp`) | Duplicates a file under a new name | Both files existed afterwards |
| Move / rename file (`mv`) | Renames or moves a file | The old name disappeared and the new name appeared |
| Display file contents (`cat`) | Prints the file's contents | Showed the text hello that I had added to the file |

### Task 2.2: Safe file changes
I created a folder named `terminal-practice`, made `notes.txt` with one line, added a second line without removing the first, displayed the file to confirm both lines were there, then made a backup copy and renamed it to `backup-notes.txt`.

- **Replacing vs adding to the end:** Using `>` replaces everything in the file, while `>>` adds new text at the end and keeps the old text.
- **Copying vs moving:** Copying leaves the original file and creates a second one. Moving relocates or renames the file, so only one remains.
- **Current-directory display:** `pwd` shows the full path of the folder I am in, so I know where my commands will act.
- **Why directory listing is useful:** `ls` shows which files and folders exist, so I can check my work and find things.

### Task 2.3: Flags and pipes
- **Flags:** `ls` shows only names. `ls -lah` shows a detailed view (`-l`), includes hidden files like `.git` (`-a`), and shows sizes in readable units like KB (`-h`). A flag changes how a command behaves.
- **Pipe:** I ran `ls -lah | head -n 5`. The pipe `|` sends the output of the command on its left into the command on its right. Here `ls -lah` produces the full listing and `head -n 5` displays only the first 5 lines.

### Task 2.4: Package managers
Command run: `brew --version` → [Homebrew version, or "brew: command not found"]
Command run: `brew list` → [short note on what it showed, or "not run because Homebrew is not installed"]

A package manager installs, updates and removes software from the command line. It saves time because it downloads the correct version and also handles other software that the program depends on.
