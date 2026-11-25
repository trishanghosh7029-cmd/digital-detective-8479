# Mission 2 — Terminal and file management

## 1. Task / objective

Practise basic Terminal commands, create and manage files safely, compare flags and pipes, and understand package managers.

## 2. Work completed

Created `terminal-practice/practice.txt` with two lines, copied it, renamed the copy, and compared file operations.

### Command reference

| Operation / command | What it does | What I observed |
|---|---|---|
| `pwd` | Prints the full absolute path of the current folder. | The path points to the assignment folder. |
| `ls` | Lists names in the current directory. | Mission folders and root files were visible. |
| `ls -l` | Displays a detailed list. | Permissions, owner fields, size and modification date appeared. |
| `cd ..` | Moves to the parent directory. | The working location changed one level upward. |
| `mkdir` | Creates a directory. | `terminal-practice` was created inside the repository. |
| `touch` | Creates an empty file or updates a timestamp. | An empty practice file was available to edit. |
| `cp` | Copies a file while keeping the original. | A backup copy could be opened without changing the original. |
| `mv` | Moves or renames a file. | The copied file name changed successfully. |
| `cat` | Displays a text file's contents. | Both original text lines were visible. |

### Safe practice answers

- Replacing a file's contents means opening it in a mode that writes over existing data. Adding text with append mode leaves existing lines and writes more data at the end.
- Copying creates a second file while preserving the original. Moving changes a file's location or name and removes it from its previous location unless a copy is created.
- `pwd` displays the absolute location of the current working directory.
- Directory listing is useful for seeing available files and folders, checking names and inspecting details such as permissions or modification dates.

### Flags and pipes

- `ls -l` adds detailed permission, owner, size and date information.
- `ls -la` also includes hidden files and directories whose names begin with a dot.
- `ls -lh` uses human-readable units for file sizes.

A pipe (`|`) sends standard output from the command on its left to the command on the right. For example, `ls -la | head -n 10` sends the first ten lines of the detailed listing to `head`, rather than displaying the entire list.

### Package manager

Homebrew was available in this environment. Its version was checked with `brew --version`; the observed version was Homebrew 7.0.9. No package was installed or removed. A package manager locates, installs, updates and removes packages while tracking their versions and dependencies. It is useful because it makes software maintenance repeatable and easier to manage.

## 3. Commands / tools used

- `pwd`, `ls`, `ls -l`, `ls -la`, `ls -lh`
- `cd`, `mkdir`, `touch`, `cp`, `mv`, `cat`
- `head` and the `|` pipe operator
- `brew --version` to check Homebrew availability
- VS Code or a text editor for file contents

## 4. My understanding

The Terminal is a direct interface to the operating system. Relative operations depend on the current directory, while absolute paths identify an exact location. Flags change command behavior, and pipes join small tools into one workflow. Safe practice should remain inside the repository and should not change system files.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- [terminal-practice/practice.txt](terminal-practice/practice.txt)
- [terminal-practice/practice-backup.txt](terminal-practice/practice-backup.txt)

## 8. Commit details

- Meaningful commit message: `Complete Terminal and file management mission`