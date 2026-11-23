# 11 - Advanced Git

## 📋 Section Overview
Advanced developer workflows: interactive history rewriting, automated bug hunting with binary search, multi-worktree execution, Git submodules, and client/server hooks.

## 🎯 Topic Checklist
- [ ] **Interactive Rebasing (`git rebase -i`)**
  - [ ] Rebasing commands: `pick`, `reword`, `edit`, `squash`, `fixup`, `drop`
  - [ ] Reordering commits and splitting a single commit into multiple commits
  - [ ] Resolving rebase conflicts (`--continue`, `--skip`, `--abort`)
  - [ ] Rebasing onto another branch (`git rebase --onto`)
- [ ] **Cherry-Picking Commits (`git cherry-pick`)**
  - [ ] Applying individual commits across disparate branches
  - [ ] Cherry-picking commit ranges
  - [ ] Resolving cherry-pick conflicts
- [ ] **Automated Bug Hunting (`git bisect`)**
  - [ ] Binary search concept in commit history
  - [ ] Manual bisect: `git bisect start`, `git bisect bad`, `git bisect good`
  - [ ] Automated bisect script execution (`git bisect run <test-script>`)
  - [ ] Cleaning up bisect state (`git bisect reset`)
- [ ] **Deep History Forensics**
  - [ ] Line-by-line attribution (`git blame -L`, ignoring whitespace with `-w`)
  - [ ] Pickaxe search: finding when a code string was added or removed (`git log -S "<string>"`)
  - [ ] Regex diff search (`git log -G "<pattern>"`)
  - [ ] Fast text searching inside commit objects with `git grep`
- [ ] **Multi-Worktrees (`git worktree`)**
  - [ ] Working on multiple branches concurrently without cloning twice
  - [ ] Adding, listing, and pruning worktrees (`git worktree add`, `list`, `prune`)
- [ ] **Submodules & Subtrees**
  - [ ] Adding and initializing submodules (`git submodule add`, `init`, `update`)
  - [ ] Updating submodule pointers vs cloning submodules recursively
  - [ ] Git subtree comparison: advantages and trade-offs
- [ ] **Git Hooks Automation**
  - [ ] Client-side hooks (`pre-commit`, `commit-msg`, `pre-push`)
  - [ ] Integrating Husky & lint-staged for JavaScript/TypeScript repositories
  - [ ] Server-side hooks (`pre-receive`, `update`)
- [ ] **Plumbing vs Porcelain Commands**
  - [ ] High-level porcelain (`add`, `commit`, `checkout`) vs low-level plumbing
  - [ ] Inspecting objects: `git cat-file -p`, `git cat-file -t`
  - [ ] Manual commit tree construction: `git write-tree`, `git commit-tree`
