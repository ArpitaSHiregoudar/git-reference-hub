# 03 - Essential Commands

## 📋 Section Overview
The day-to-day command kit required for authoring, staging, committing, inspecting, and navigating repository history.

## 🎯 Topic Checklist
- [ ] **Staging Operations (`git add`)**
  - [ ] Staging individual files vs entire directories (`git add .`)
  - [ ] Interactive patch staging (`git add -p` / `--patch`)
  - [ ] Adding modified files while ignoring untracked (`git add -u`)
- [ ] **Commit Crafting (`git commit`)**
  - [ ] Anatomy of an effective commit message
  - [ ] Conventional Commits specification (`feat:`, `fix:`, `docs:`, `refactor:`, `chore:`)
  - [ ] Inline messages vs editor multi-line messages
  - [ ] Staging and committing in one step (`git commit -am`)
- [ ] **History Inspection (`git log`)**
  - [ ] Concise single-line log graphs (`git log --oneline --graph --decorate --all`)
  - [ ] Filtering history by author, date, file path, and commit message regex
  - [ ] Showing commit stats and changed lines (`git log --stat`, `git log --patch`)
- [ ] **Diffing Changes (`git diff`)**
  - [ ] Working tree vs Staging area (`git diff`)
  - [ ] Staging area vs Last commit (`git diff --staged` / `git diff --cached`)
  - [ ] Comparing specific commits, tags, or branches
  - [ ] Word-level diffs (`--word-diff`)
- [ ] **File Operations Inside Git**
  - [ ] Safe renaming and tracking with `git mv`
  - [ ] Removing tracked files with `git rm`
  - [ ] Cleaning untracked files safely (`git clean -ndf`, `git clean -df`)
