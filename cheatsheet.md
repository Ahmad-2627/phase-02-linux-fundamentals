# 🐧 Phase 2 — Linux Fundamentals: Cheat Sheet

## Navigation
| Command | What it does |
|---|---|
| `pwd` | Show current folder location |
| `ls` | List files/folders here |
| `ls -l` | List with details (permissions, owner, size) |
| `ls -a` | Show hidden files too |
| `cd foldername` | Move into a folder |
| `cd ..` | Move up one level |
| `cd ~` or `cd` | Go to home folder |
| `cd /` | Go to root (top of file system) |

## File & Directory Management
| Command | What it does |
|---|---|
| `mkdir name` | Create a new folder |
| `touch file.txt` | Create a new empty file |
| `cat file.txt` | Show file contents |
| `cp source dest` | Copy a file |
| `cp -r source dest` | Copy a folder |
| `mv source dest` | Move or rename a file/folder |
| `rm file` | Delete a file (permanent, no undo) |
| `rm -r folder` | Delete a folder and everything inside |
| `echo "text" > file` | Write text into a file (overwrites) |
| `echo "text" >> file` | Add text to end of file (doesn't overwrite) |

## File Permissions
| Command | What it does |
|---|---|
| `ls -l` | View permissions of files |
| `chmod 755 file` | Set permissions (owner=7, group=5, others=5) |
| `chmod +x file` | Make a file executable |
| `chown user file` | Change file owner |
| `chown user:group file` | Change owner and group |

**Permission numbers:** `r=4, w=2, x=1` → add them up per group (owner/group/others)

**SUID reminder:** `chmod 777` = wide open access. **SUID** = program runs as its owner's identity, no matter who runs it. Different problems, don't confuse them.

## Users & Groups
| Command | What it does |
|---|---|
| `whoami` | Show current username |
| `id` | Show your UID, GID, and groups |
| `groups` | List groups you belong to |
| `sudo command` | Run a command as root (superuser) |
| `cat /etc/passwd` | List all users |

## Processes & Services
| Command | What it does |
|---|---|
| `ps aux` | Show all running processes |
| `top` | Live view of processes (press `q` to quit) |
| `kill PID` | Stop a process by its ID number |
| `systemctl status name` | Check if a service is running |
| `sudo systemctl start name` | Start a service |
| `sudo systemctl stop name` | Stop a service |

## Package Management (apt)
| Command | What it does |
|---|---|
| `sudo apt update` | Refresh list of available packages |
| `sudo apt upgrade` | Update all installed packages |
| `sudo apt install toolname` | Install new software |
| `sudo apt remove toolname` | Uninstall software |
| `apt search keyword` | Search for a package |

## SSH — Remote Access
| Command | What it does |
|---|---|
| `ssh user@ip` | Connect to a remote machine |
| `ssh-keygen` | Generate a key pair for passwordless login |
| `scp file user@ip:/path` | Securely copy a file to a remote machine |
| `sudo systemctl start ssh` | Start SSH service on your own machine |

## Bash Scripting
```bash
#!/bin/bash              # shebang - tells Linux to run this with Bash
echo "Hello, Ahmad"       # prints text
name="value"               # variable
echo "$name"                # use a variable
```
| Command | What it does |
|---|---|
| `nano script.sh` | Open/create a script in text editor |
| `chmod +x script.sh` | Make script executable |
| `./script.sh` | Run the script |

---

Noted your full instructions and preferences (simple English, tech terms explained, roadmap remembered across chats). This matches what we've been doing — no changes needed. Ready for Phase 3 whenever you are.
