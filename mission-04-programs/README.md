# Mission 4 — How programs run

## 1. Task / objective
Run a simple Python program and compare how compilers and interpreters translate or execute programs.

## 2. Work completed

### Task 4.1: Python program
I created a file named `hello.py` in this folder with one line that prints a message. I saved it and ran it with `python3 hello.py`. The message "Hello from Python" appeared in the Terminal, so the program worked.

### Task 4.2: Compiler vs interpreter

| Point | Compiler | Interpreter |
|---|---|---|
| When translation / execution happens | Translates the whole program into machine code before it runs | Reads and runs the program line by line while it is running |
| Typical output | A separate executable file | No separate file, the result appears directly as the program runs |
| One example | C compiler (gcc) | Python interpreter |
| One advantage | The compiled program usually runs faster | Easy to test and fix quickly, since code can be run right away |

**Difference in my own words:** A compiler translates the complete source code into machine code first, and only after that can the program be run. An interpreter does not make a separate file. It reads the code and carries out each instruction while the program is running. As the table shows, compiled programs usually run faster, while interpreted programs are easier to test because I can run them immediately. Some languages, like Java, use both steps.

## 3. Commands / tools used
- `cd` – moved into the mission folder
- `touch hello.py` – created the Python file
- `python3 hello.py` – ran the program using the Python 3 interpreter
- Tools: VS Code, zsh terminal
