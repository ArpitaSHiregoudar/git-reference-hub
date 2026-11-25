# 02. Essential Settings

---

## 1. Identity (Required)

Every commit records **who** made it. Set this first:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

> ⚠️ This email must match the email on your GitHub account for your commits to be linked to your profile.

Verify:

```bash
git config user.name
git config user.email
```

---

## 2. Default Branch Name

By default, `git init` creates a branch called `master`. The industry standard is now `main`:

```bash
git config --global init.defaultBranch main
```

Now every new repo you create will start with `main` instead of `master`.

---

## 3. Default Editor

When Git needs you to write a message (e.g., during merge or rebase), it opens a text editor. The default is usually Vim, which can be confusing for beginners.

**Set VS Code as your default editor:**

```bash
git config --global core.editor "code --wait"
```

The `--wait` flag tells Git to pause until you close the editor tab.

**Other options:**

| Editor | Command |
|---|---|
| VS Code | `code --wait` |
| Nano | `nano` |
| Vim | `vim` |
| Notepad (Windows) | `notepad` |
| Notepad++ | `'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin` |

---

## 4. Line Endings (Cross-Platform Fix)

**The problem:** Windows uses `CRLF` (Carriage Return + Line Feed) for line endings, while Linux/Mac uses `LF` (Line Feed only). Without configuration, Git may show every line as changed even when only the line endings differ.

**The fix — `core.autocrlf`:**

| OS | Setting | What It Does |
|---|---|---|
| **Windows** | `git config --global core.autocrlf true` | Converts LF → CRLF when checking out, CRLF → LF when committing. |
| **Mac / Linux** | `git config --global core.autocrlf input` | Converts CRLF → LF when committing. No conversion on checkout. |

```bash
# On Windows:
git config --global core.autocrlf true

# On Mac/Linux:
git config --global core.autocrlf input
```

> **Why this matters:** It ensures your repository always stores files with `LF` endings (the universal standard) regardless of which OS each team member uses.

---

## 5. Git Aliases (Shortcuts)

Aliases let you create short custom commands for things you type often.

### Setting Aliases

```bash
git config --global alias.s "status"
git config --global alias.co "checkout"
git config --global alias.br "branch"
git config --global alias.cm "commit -m"
git config --global alias.lg "log --oneline --graph --all --decorate"
```

### Using Them

```bash
git s          # Same as: git status
git co main    # Same as: git checkout main
git cm "msg"   # Same as: git commit -m "msg"
git lg         # Beautiful one-line commit graph
```

### View All Aliases

```bash
git config --get-regexp alias
```

---

## 6. Color Output

Git colors are usually on by default, but you can ensure it:

```bash
git config --global color.ui auto
```

---

## Recommended Starter Config

Here's a summary of everything above in one block:

```bash
# Identity
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Defaults
git config --global init.defaultBranch main
git config --global core.editor "code --wait"
git config --global color.ui auto

# Line endings (Windows)
git config --global core.autocrlf true

# Aliases
git config --global alias.s "status"
git config --global alias.co "checkout"
git config --global alias.br "branch"
git config --global alias.cm "commit -m"
git config --global alias.lg "log --oneline --graph --all --decorate"
```

---

## 🎯 Interview Ready

**Q: What is the first thing you configure after installing Git?**
> Your identity — `user.name` and `user.email` — because Git embeds this information into every commit. Without it, Git will refuse to commit or use a placeholder.

**Q: What does `core.autocrlf` do and why is it important?**
> It controls automatic line ending conversion between Windows (CRLF) and Linux/Mac (LF). Setting it properly ensures consistent line endings in the repository regardless of which operating system each developer uses, preventing unnecessary diffs caused by line ending differences.

**Q: What is a Git alias?**
> A Git alias is a custom shortcut for a longer Git command, stored in your config file. For example, `alias.s = status` lets you type `git s` instead of `git status`.

---

> **Next →** [03-ssh-and-authentication.md](./03-ssh-and-authentication.md) — Set up SSH keys and authentication for GitHub.
