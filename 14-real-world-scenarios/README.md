# 14 - Real-World Scenarios

## 📋 Section Overview
Field-tested triage runbooks for handling common Git disasters, panicked moments, accidental commits, and broken team repositories.

## 🎯 Topic Checklist
- [ ] **Scenario 01: Committed Directly to `main` Instead of a Feature Branch**
  - [ ] How to move those unpushed commits to a new branch and restore clean `main`
- [ ] **Scenario 02: Committed Secrets/Credentials into Repository History**
  - [ ] Immediate invalidation & rotation of leaked keys
  - [ ] Removing sensitive files from recent commits vs rewriting entire Git history (`git-filter-repo` / BFG Repo-Cleaner)
  - [ ] Force pushing the scrubbed history safely
- [ ] **Scenario 03: Emergency Hotfix While Midst an Unfinished Feature**
  - [ ] Stashing uncommitted work safely (`git stash -u`)
  - [ ] Cutting hotfix from production tag/branch, testing, and shipping
  - [ ] Resuming feature work without conflict (`git stash pop`)
- [ ] **Scenario 04: Feature Branch Diverged 50+ Commits Behind `main`**
  - [ ] Deciding between merging `main` into feature vs interactive rebase onto `main`
  - [ ] Chunking conflict resolution step-by-step
- [ ] **Scenario 05: Ran `git reset --hard` and Lost Unpushed Commits**
  - [ ] Finding lost commit hashes via `git reflog`
  - [ ] Rebuilding the branch state in seconds
- [ ] **Scenario 06: Combining 10+ Chaotic "WIP / fix typo" Commits into One**
  - [ ] Squash rebase (`git rebase -i HEAD~10`)
  - [ ] Reset soft technique (`git reset --soft origin/main && git commit`)
- [ ] **Scenario 07: Need to Split One Massive Commit into Two Atomic Commits**
  - [ ] Using `git rebase -i` with `edit` command
  - [ ] Unstaging with `git reset HEAD~` and staging selective hunks
- [ ] **Scenario 08: Trapped in a Detached HEAD State**
  - [ ] Understanding why `HEAD` detached
  - [ ] Saving experimental work into a named branch before switching away
