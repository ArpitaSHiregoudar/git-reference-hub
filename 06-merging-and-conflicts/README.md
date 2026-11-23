# 06 - Merging and Conflicts

## 📋 Section Overview
Understand the algorithmic mechanics of Git merges, dissect merge conflicts down to marker anatomy, and master conflict resolution workflows.

## 🎯 Topic Checklist
- [ ] **Merge Mechanics & Algorithms**
  - [ ] Fast-forward merge (linear pointer advance)
  - [ ] Three-way merge (common ancestor, recursive / `ort` merge strategy)
  - [ ] Explicit non-fast-forward merge (`git merge --no-ff`)
  - [ ] Squash merge (`git merge --squash`): pros, cons, and when to use
- [ ] **Conflict Anatomy & Markers**
  - [ ] Why conflicts occur: concurrent edits to identical lines
  - [ ] Reading conflict markers (`<<<<<<< HEAD`, `=======`, `>>>>>>> <branch>`)
  - [ ] Diff3 conflict style (`merge.conflictStyle diff3` or `zdiff3`) to see the ancestor base
- [ ] **Conflict Resolution Workflows**
  - [ ] Manual resolution: editing, removing markers, staging, and completing
  - [ ] Visual merge tools (`git mergetool`, VS Code 3-way editor)
  - [ ] Resolving using strategy options (`-X ours` vs `-X theirs`)
  - [ ] Aborting a conflicted merge cleanly (`git merge --abort`)
- [ ] **Reuse Recorded Resolution (`git rerere`)**
  - [ ] What is `rerere` and how it saves time on long-lived rebased branches
  - [ ] Enabling `rerere.enabled true`
  - [ ] Automatic recording and replay of conflict resolutions
