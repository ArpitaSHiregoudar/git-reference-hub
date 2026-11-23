# 01 - Git Fundamentals

## 📋 Section Overview
This module explores version control from first principles, establishing the mental model and architecture that powers Git under the hood.

## 🎯 Topic Checklist
- [ ] **Core Concepts**
  - [ ] What is Version Control? (CVCS vs DVCS comparison)
  - [ ] Why Git won: speed, data integrity, distributed workflow
  - [ ] Snapshots vs Deltas: How Git models repository history
- [ ] **Git Architecture & The Three Trees**
  - [ ] Working Directory (untracked & modified files)
  - [ ] Staging Area / Index (prepared snapshots)
  - [ ] Repository / Commit History (immutable object graph)
  - [ ] Remote tracking & distributed synchronization
- [ ] **The Git Object Database Internals**
  - [ ] Content-Addressable Storage (SHA-1 / SHA-256 hashes)
  - [ ] Blobs (file contents, compression)
  - [ ] Trees (directory structure & file naming)
  - [ ] Commits (metadata, author, committer, parent pointer)
  - [ ] Annotated Tags (permanent reference objects)
- [ ] **Hands-on Initiation**
  - [ ] Initializing a fresh repository (`git init`)
  - [ ] Inspecting the hidden `.git` folder structure (`objects`, `refs`, `HEAD`, `config`)
  - [ ] Checking repository state with `git status`
  - [ ] Creating and inspecting the first commit
