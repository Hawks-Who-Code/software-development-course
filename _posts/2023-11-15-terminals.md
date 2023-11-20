---
layout: post
title: The Development Environment Pt. 2 - Terminals
date: 2023-11-15
tags: general-skills the-development-environment
---

# A little bit of history

The first personal computers did not have a mouse or graphical user interface. The only way to use them was through the terminal--entering commands to navigate the computer and run programs

# What are terminals?

- Allows us to talk to our computer directly
- Like the desktop
- Like the file explorer

Terminals can have different “shells” which are different programs to communicate with the computer but can come with different features or commands. Different operating systems often have completely different commands and directory structures.

Linux will often use bash where Windows uses Command Prompt but more often now, Powershell.

Though you will see linux if you work professionally, windows is more common for many hobbyists and it is what we have access to now, so we will use Powershell today.

# The Windows directory structure

```txt
C:\
  Program Files\
  Program Files (x86)\
  Users\
    Exampleuser1\
      AppData\
      Desktop\
      Documents\
      Downloads\
      Pictures\
      Start Menu\
    Exampleuser2\
    Exampleuser3\
  Windows\
```

# Navigating the terminal

You will begin in the home directory which will be set to your user folder.

**Absolute paths** include the entire path starting from the root directory.
**Relative paths** are paths that start relative to your current directory.

| . | Current |
| .. | Parent |
| ~ | Home |
| \ | Root |

| Alias | Real command | Description |
| cd <directory> | Set-Location | Change directory |
| ls <directory> | Get-ChildItem | List files and directories |
| cat <file> | Get-Content | View the contents of a file |
| mv <from> <to> | Move-Item | Move item |
| cp  <from> <to> | Copy-Item | Copy item |
| rm <file> | Remove-Item | Delete item |
| wget <url> | Invoke-WebRequest | Download from the web |
| help <command> | Get-Help | Get help with a command |


Use quotes if the filename has spaces.
To run an executable file, just put in the file path
Use tab to autocomplete commands

# Flags

Flags modify how a command runs. Each command has its own set of flags that can be set and configured.

Flags are set on the same line as running the command, following the command’s main body, e.g. “rm <file> -Recurse”.

| Flag | Command | Operation |
| -Recurse | cp or rm | Operate on a folder |
| -Tail <num> | cat | Only read the end of a file |

# Activity

- Open Powershell by hitting the windows command button then typing “Powershell” to find the app
- Try navigating to a directory with system level program files
- Try opening notepad from the command line to make a new file
- Try renaming a file
- Try opening a Chrome window from the terminal
- Try downloading a GitHub repository from the terminal
