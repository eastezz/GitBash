# Run Programs with Git Bash & Create Custom Bash Commands

This tutorial explains how to:

* Run Windows programs using **Git Bash**
* Create your own **custom terminal commands**
* Automatically open programs like **Visual Studio** from the terminal

The tutorial is beginner-friendly and works on Windows.


# 1. What is Git Bash?

Git Bash is a terminal emulator that comes with **Git for Windows** and provides a Unix-like command line environment on Windows.

It allows you to run:

* Linux-like commands (`ls`, `cd`, `grep`, etc.)
* Git commands
* Windows executables

Example terminal:

```
MINGW64 ~/Projects
$
```


# 2. Running Windows Programs from Git Bash

In Git Bash, Windows drives are mapped like this:

| Windows Path | Git Bash Path |
| ------------ | ------------- |
| `C:\`        | `/c/`         |
| `D:\`        | `/d/`         |

Example:

Windows path:

```
C:\Program Files\App\app.exe
```

Git Bash path:

```
/c/Program Files/App/app.exe
```

Run the program:

```bash
"/c/Program Files/App/app.exe"
```

Quotes are required when the path contains spaces.


# 3. Example: Running Visual Studio

Example command:

```bash
"/c/Program Files/Microsoft Visual Studio/2022/Community/Common7/IDE/devenv.exe"
```

You can also open a solution file:

```bash
"/c/Program Files/Microsoft Visual Studio/2022/Community/Common7/IDE/devenv.exe" MyProject.sln
```


# 4. Creating Your Own Bash Commands (Aliases)

Aliases allow you to create **short commands** for long commands.

Example:

Instead of typing a long path every time, create a shortcut.

### Step 1: Open `.bashrc`

```bash
nano ~/.bashrc
```


### Step 2: Add a custom command

Example alias:

```bash
alias vs='"/c/Program Files/Microsoft Visual Studio/2022/Community/Common7/IDE/devenv.exe"'
```

Now you can run:

```bash
vs
```


# 5. Reload Bash Configuration

After editing `.bashrc`, reload it:

```bash
source ~/.bashrc
```

Now your command works immediately.


# 6. Useful Custom Commands

### Open current folder in Visual Studio

```bash
alias vs='"/c/Program Files/Microsoft Visual Studio/2022/Community/Common7/IDE/devenv.exe" .'
```

Usage:

```bash
vs
```

### Open VS Code

```bash
alias code='"/c/Users/USERNAME/AppData/Local/Programs/Microsoft VS Code/Code.exe"'
```

### Quick navigation

```bash
alias projects='cd ~/Projects'
```

Usage:

```bash
projects
```

# 7. Where Bash Commands Are Stored

Your custom commands are stored in:

```
~/.bashrc
```

Location example:

```
C:\Users\YourUser\.bashrc
```

Every time Git Bash starts, this file is executed.

# 8. Tips for Better Terminal Workflow

* Use `alias` to shorten long commands
* Create navigation shortcuts
* Launch programs directly from the terminal
* Automate repetitive tasks

Example:

```bash
alias run='gcc main.c -o main && ./main'
```


