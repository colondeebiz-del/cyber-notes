# Linux Command Foundations

This document serves as a long-term reference for Linux command-line usage.
It is intended to be revisited regularly to build familiarity, confidence 
and memory over time.

# How to Learn Commands You Don't Know

If you want to learn commands you don't know, this is 
what you'd type into your terminal: 

man <command>

Or:

<command> --help

Example:

man ls

Or:

grep --help

This is how most people learn commands outside of googling it.
---

## 1. What is a Linux Command?

Most Linux commands follow this structure:

command [options] [arguments]

Example:

ls -la /etc

```
- ls   →  the command (what you are telling the terminal to do.) 
- -la  →  options (flags that modify behavior)
- /etc →  argument (the target)

This structure is the main thing i want to keep in mind when inside the 
terminal.
```

## 2. The Command Glossary

### Core Navigation and File Commands

```

pwd          # show current directory
ls           # list directory contents
cd           # change directory
tree         # show directory tree (if installed)

touch        # create empty file
mkdir        # create directory
rm           # remove file or directory
rmdir        # remove empty directory
cp           # copy files/directories
mv           # move or rename
stat         # detailed file info

```
####  Viewing and Reading Files

```

cat          # print file contents
less         # paginated file viewer
head         # first lines of a file
tail         # last lines of a file
tail -f      # follow file updates (logs)
wc           # word/line/byte counts

```
#### Searching and Text-Processing

```

grep         # search text by pattern
find         # search filesystem
awk          # structured text processing
sed          # stream editor
cut          # extract columns
sort         # sort output
uniq         # remove duplicates

--- These commands are frequently chained together using pipes*

```

pipes contextual definition: 

pipes example:
```

command1 | command2 | command3


```
#### Permissions and Ownership

```

chmod        # change permissions
chown        # change owner
chgrp        # change group
umask        # default permission mask

```
--- Permisions example format:
```

-rxr-xr--

```
#### Processes and System State
```

ps           # process list
top          # live process monitor
htop         # enhanced process monitor (if installed)
kill         # send signal to process
killall      # kill process by name
uptime       # system uptime and load
free         # memory usage
df -h        # disk usage
du -sh       # directory size

```
#### Networking Fundamentals (the idea is for these to be Security-relevant)
```

ip a         # network interfaces
ip r         # routing table
ss           # socket statistics
ping         # reachability test
curl         # HTTP requests
wget         # file download
nc           # netcat (raw network connections)

```
#### Package Management (Ubuntu Specific)
```

apt update
apt upgrade
apt install
apt remove
apt search

```
#### Users, Privileges, and Identities
```

whoami
id
groups
passwd
su
sudo

```
#### Shell and Environment
```

history
clear
alias
env
export
which
type

```
#Notes updates
- 01/06/2026: Daily Drills created and added the how to workflow to combat shortened attention span in Personal Notes.


# Personal Notes Section

--- 
How to actually run the drills:

1. Open a Terminal (ctrl + shift + T)

2. Navigate to cyber-notes repo

```

cd ~/cyber-notes

```

3. Open the drill file for reference

```

ip a
ss -tuln
ping -c 3 8.8.8.8

```
4. run the commands manually in another terminal tab/window ( Ctrl + Shift + N )
