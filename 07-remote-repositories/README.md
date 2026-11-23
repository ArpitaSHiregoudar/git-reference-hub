# 07 - Remote Repositories

## 📋 Section Overview
Manage distributed collaboration channels, understand remote tracking branches, master synchronization commands, and prune stale references.

## 🎯 Topic Checklist
- [ ] **Understanding Remote References**
  - [ ] What is an `origin`? How remotes are defined in `.git/config`
  - [ ] Local branches vs Remote tracking branches (`origin/main`, `refs/remotes/`)
  - [ ] Listing and inspecting remotes (`git remote -v`, `git remote show origin`)
  - [ ] Adding, renaming, and removing remotes (`git remote add`, `rename`, `remove`)
- [ ] **Synchronizing History**
  - [ ] `git fetch`: downloading objects without altering the working tree
  - [ ] `git pull`: fetch + merge vs `git pull --rebase`
  - [ ] Upstream tracking configuration (`git push -u origin <branch>` / `--set-upstream`)
  - [ ] Force pushing safely: why `git push -f` is dangerous and why `git push --force-with-lease` is mandatory
- [ ] **Managing Tags on Remotes**
  - [ ] Lightweight vs Annotated tags (`git tag -a v1.0.0 -m "Release"`)
  - [ ] Pushing individual tags vs all tags (`git push origin <tag>`, `git push --tags`)
  - [ ] Deleting tags locally and remotely (`git tag -d`, `git push origin --delete <tag>`)
- [ ] **Remote Hygiene & Housekeeping**
  - [ ] Pruning deleted remote branches (`git fetch --prune` / `git remote prune origin`)
  - [ ] Configuring automatic pruning (`git config --global fetch.prune true`)
  - [ ] Working with dual remotes (`origin` for fork, `upstream` for original repo)
