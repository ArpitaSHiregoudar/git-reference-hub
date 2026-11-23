# 10 - Git Undo Magic

## 📋 Section Overview
The definitive survival guide to rewinding time, rescuing deleted commits, repairing corrupted states, and stashing work safely in Git.

## 🎯 Topic Checklist
- [ ] **Undoing Uncommitted Changes**
  - [ ] Discarding working directory edits (`git restore <file>` vs legacy `git checkout -- <file>`)
  - [ ] Unstaging files from the index (`git restore --staged <file>` vs legacy `git reset HEAD <file>`)
  - [ ] Interactive selective discards (`git restore -p`)
- [ ] **Amending Recent Commits**
  - [ ] Modifying the last commit message or files (`git commit --amend`)
  - [ ] Preserving author timestamp with `--no-edit`
  - [ ] Golden Rule: Never amend commits already pushed to shared public branches
- [ ] **The Deep Reset Spectrum (`git reset`)**
  - [ ] Soft reset (`--soft`): rewinding commit pointer while keeping index and working tree
  - [ ] Mixed reset (`--mixed`, default): rewinding commit pointer and index, keeping working tree
  - [ ] Hard reset (`--hard`): completely wiping commits, index, and uncommitted working tree
- [ ] **Safe Public Reversals (`git revert`)**
  - [ ] How `git revert` creates forward undo commits
  - [ ] Reverting single commits vs ranges of commits
  - [ ] Reverting merge commits (`git revert -m 1 <commit-hash>`)
- [ ] **The Ultimate Safety Net: `git reflog`**
  - [ ] Understanding reference logs: where every `HEAD` movement is recorded
  - [ ] Recovering deleted branches and commits lost after `git reset --hard`
  - [ ] Time-based navigation (`HEAD@{1.day.ago}`, `HEAD@{2}`)
- [ ] **Stashing for Context Switching (`git stash`)**
  - [ ] Stashing modified and untracked files (`git stash -u`)
  - [ ] Inspecting stash contents (`git stash list`, `git stash show -p`)
  - [ ] Applying, popping, and dropping stashes (`git stash pop`, `git stash apply`, `git stash drop`)
  - [ ] Converting a stash into a branch (`git stash branch <name>`)
