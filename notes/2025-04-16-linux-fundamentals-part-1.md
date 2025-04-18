# 🐧 TryHackMe: Linux Fundamentals Part 1  
**Date:** 2025-04-16  
**Room:** https://tryhackme.com/room/linuxfundamentalspart1  
**Status:** ✅ Completed  

---

## 🧭 Task 1: Getting Started

Jumped into the first room of the Linux Fundamentals series. No expectations to know anything going in — good, because I didn't. Just started getting familiar with the layout and flow of THM rooms.

---

## 📚 Task 2: Background on Linux

Quick overview of what Linux is:

- Unix-like, open-source OS
- Created by Linus Torvalds in 1991
- Major selling points: security, flexibility, performance, and total control

Common distros mentioned: Ubuntu, Kali, Fedora. I'm seeing why Linux is the OS of choice for security folks and hackers — it’s minimal but powerful.

---

## 🖥️ Task 3: My First Linux Machine

Spawned my first TryHackMe Linux machine (Ubuntu). This was more about observation than interaction. Just getting used to the idea that everything happens through the terminal.

---

## 🔧 Task 4: First Commands

Ran a few basic commands:

- `echo "TryHackMe"` — Just prints whatever you put in quotes. Easy start.
- `whoami` — Shows the current user I’m logged in as.

Getting the feel for shell interaction. Commands are short and to the point — no fluff, just results.

---

## 📂 Task 5: Filesystem Basics

Spent time exploring the Linux file system. Commands I used:

- `ls` — Lists everything in the current folder
- `cd foldername` — Change directory into a folder
- `cat file.txt` — View the contents of a file
- `pwd` — Shows where I am in the filesystem (absolute path)

Practically speaking, I was asked to:
- Count how many folders were in `/home/tryhackme`
- Find which folder had a file inside
- Output the contents of that file using `cat`

This helped reinforce how navigation in Linux works — you really do have to keep track of where you are at all times.

---

## 🔍 Task 6: Finding Files

Started working with `find` and `grep`:

- `find -type f -name filename` — Locates a file by name
- `grep "text" filename` — Searches inside a file for matching text

I had to find a specific log file (`access.log`) and search it for the word `THM`. Got the flag using:

```bash
grep "THM" access.log
```

The `find` command honestly felt powerful once I understood the syntax — it’ll definitely come in handy later.

---

## 🔧 Task 7: Shell Operators

This section covered redirection and chaining commands:

- `>` — Overwrites a file with output
- `>>` — Appends output to the file
- `&&` — Run the second command **only if** the first succeeds
- `&` — Runs the command in the background (not relevant now, but noted)

Example:
```bash
echo password123 > passwords     # Replaces content
echo tryhackme >> passwords      # Appends new line
```

This stuff is basic shell scripting 101 — powerful even at this level.

---

## 🧠 Task 8: Wrapping Up

Finished the room with a quick recap of everything I touched:

- Terminal basics
- Filesystem navigation
- Working with files
- Finding stuff
- Output redirection and logic chaining

The room made it clear: Linux is less about memorizing and more about thinking in **steps**. Every command is a tool. Knowing when to use what is the skill I’m building.

---

## 🏁 Notes to Myself

- Linux isn’t hard, but it *does* demand patience.
- Navigation and observation are key.
- Practicing these core commands is gonna make everything easier later — in security labs, CTFs, and real-world troubleshooting.

---

## ✅ Room Complete

That’s a wrap on Part 1. It’s foundational, but I feel like it already gave me a mental map for how Linux “thinks.” Moving on to Part 2 with way more confidence than I had an hour ago.
