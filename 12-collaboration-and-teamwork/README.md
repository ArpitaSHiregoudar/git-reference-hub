# 12 - Collaboration and Teamwork

## 📋 Section Overview
Patterns and standards for cross-functional engineering teams, open source contribution, repository governance, and frictionless code ownership.

## 🎯 Topic Checklist
- [ ] **Open Source & Forking Workflows**
  - [ ] Upstream repository vs Origin fork model
  - [ ] Adding and keeping the upstream remote in sync (`git fetch upstream && git merge upstream/main`)
  - [ ] Pushing to personal fork and opening cross-repository pull requests
- [ ] **Team Commit Standards & Conventions**
  - [ ] Conventional Commits specification (structure, types, breaking changes `!`)
  - [ ] Semantic versioning connection (`fix` = patch, `feat` = minor, `BREAKING CHANGE` = major)
  - [ ] Gitmoji conventions and commit clarity
- [ ] **Pair Programming & Co-Authorship**
  - [ ] Adding co-authors to commit trailers (`Co-authored-by: Name <email>`)
  - [ ] Multi-author verification on GitHub commit history
- [ ] **Code Ownership with `CODEOWNERS`**
  - [ ] Defining `.github/CODEOWNERS` syntax
  - [ ] Path-based team and user reviewer assignments
  - [ ] Mandatory code owner review policies
- [ ] **Collaborative Conflict Prevention**
  - [ ] Communication patterns for feature branches
  - [ ] Preventing merge train bottlenecks with frequent rebasing / fast-forwarding
  - [ ] Team guidelines for avoiding long-lived branch divergence
