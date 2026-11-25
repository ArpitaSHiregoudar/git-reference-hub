# 01 - Git Fundamentals

## 📋 Section Overview
This module explores version control from first principles, establishing the mental model and architecture that powers Git under the hood.

## 🎯 Topic Checklist
- [ ] **Core Concepts**
  - [x] [What is Version Control? (CVCS vs DVCS comparison)](./01-what-is-version-control.md)
  - [ ] Why Git won: speed, data integrity, distributed workflow
  - [ ] Snapshots vs Deltas: How Git models repository history
- [x] **Git Architecture & The Three Trees** — *See [git_architecture.md](./git_architecture.md)*
  - [x] [Working Directory (untracked & modified files)](./git_architecture.md#1-the-working-directory-the-sandbox)
  - [x] [Staging Area / Index (prepared snapshots)](./git_architecture.md#2-the-staging-area--the-index-the-launchpad)
  - [x] [Repository / Commit History (immutable object graph)](./git_architecture.md#3-the-local-repository-the-permanent-vault)
  - [x] [Remote tracking & distributed synchronization](./git_architecture.md#part-1-the-three-areas-the-three-trees-architecture)
- [x] **The Git Object Database Internals** — *See [git_architecture.md](./git_architecture.md)*
  - [x] [Content-Addressable Storage (SHA-1 / SHA-256 hashes)](./git_architecture.md#part-2-the-core-object-database-the-four-sacred-objects)
  - [x] [Blobs (file contents, compression)](./git_architecture.md#1-the-blob-binary-large-object)
  - [x] [Trees (directory structure & file naming)](./git_architecture.md#2-the-tree-directory-manifest)
  - [x] [Commits (metadata, author, committer, parent pointer)](./git_architecture.md#3-the-commit-the-snapshot-envelope)
  - [x] [Annotated Tags (permanent reference objects)](./git_architecture.md#4-the-annotated-tag-the-permanent-landmark)
- [ ] **Hands-on Initiation**
  - [ ] Initializing a fresh repository (`git init`)
  - [ ] Inspecting the hidden `.git` folder structure (`objects`, `refs`, `HEAD`, `config`)
  - [ ] Checking repository state with `git status`
  - [ ] Creating and inspecting the first commit
