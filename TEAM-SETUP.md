# Deodato Shared Files — Team Setup Guide

This guide gets you set up to view, edit, and collaborate on shared Deodato files hosted on GitHub.

---

## What You Need (one-time setup)

1. **A GitHub account** — create one free at [github.com](https://github.com)
2. **Git** — download at [git-scm.com/download/win](https://git-scm.com/download/win) (Windows) or [git-scm.com/download/mac](https://git-scm.com/download/mac) (Mac). Use all default settings during install.
3. **VS Code** — download at [code.visualstudio.com](https://code.visualstudio.com)
4. **Live Share extension** — open VS Code, press `Ctrl+Shift+X`, search "Live Share", install it
5. **Send Mike your GitHub username** so he can add you as a collaborator

---

## First-Time Repo Setup

Once Mike has added you as a collaborator, you'll get an email invite — accept it, then:

**1. Clone the repo to your computer**

Open a terminal (Mac: Terminal app / Windows: Git Bash or Command Prompt) and run:

```bash
git clone https://github.com/mike-trentham/deodato-proof-points.git
cd deodato-proof-points
```

This downloads the files to your computer.

**2. Open in VS Code**

```bash
code .
```

---

## Viewing the Live File

The latest version of any file is always available at:

**`https://mike-trentham.github.io/deodato-proof-points/deodato-proof-points.html`**

Bookmark this. It updates automatically within ~60 seconds of any push.

---

## Making Edits (Solo)

1. Open VS Code in the repo folder
2. Edit the file
3. Save, then open a terminal and run:

```bash
git add .
git commit -m "brief description of your change"
git push
```

4. Wait ~60 seconds and refresh the live URL to see your changes

**Before editing, always pull the latest version first** to avoid conflicts:

```bash
git pull
```

---

## Real-Time Co-Editing (Live Share)

Use this when you and a teammate want to edit the same file simultaneously.

**To start a session (host):**
1. Open the file in VS Code
2. Click **Live Share** in the bottom status bar
3. A link is copied to your clipboard — send it to your teammate

**To join a session (guest):**
1. Click the link your teammate sent
2. VS Code opens automatically and you're both in the file
3. You'll see each other's cursors in real time

**When the session ends:**
The host commits and pushes to save changes to GitHub:
```bash
git add .
git commit -m "live session edits"
git push
```

---

## Tips

- Always `git pull` before starting work to make sure you have the latest version
- Write a short, descriptive commit message so the team knows what changed
- If you get a conflict (two people edited the same line), message Mike — he'll sort it out
- The `.html` file is what gets published; the `.docx` is just a backup source doc — don't worry about editing that

---

## Questions?

Reach out to Mike at michael@deodato.co
