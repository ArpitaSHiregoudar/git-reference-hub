# 09 - Pull Requests and Reviews

## 📋 Section Overview
The art and engineering of asynchronous code reviews: crafting readable PRs, giving constructive feedback, and configuring automated branch protection.

## 🎯 Topic Checklist
- [ ] **Crafting High-Quality Pull Requests**
  - [ ] PR sizing: why smaller, atomic PRs review 10x faster
  - [ ] Writing comprehensive descriptions: Context, Problem, Solution, Verification steps
  - [ ] Linking issues automatically (`Closes #123`, `Fixes #456`)
  - [ ] Draft PRs for early architectural feedback
- [ ] **Reviewer Mechanics & Etiquette**
  - [ ] Line-by-line review comments and batch reviews
  - [ ] Suggesting code changes directly within GitHub's diff viewer
  - [ ] Review statuses: Comment, Approve, Request Changes
  - [ ] Conventional Comments standard (`praise:`, `nitpick:`, `question:`, `suggestion:`, `blocking:`)
- [ ] **Branch Protection Rules & GitHub Rulesets**
  - [ ] Requiring pull request reviews before merging
  - [ ] Requiring status checks to pass before merging (CI gatekeeping)
  - [ ] Enforcing linear history and signed commits
  - [ ] Code owner approvals via `CODEOWNERS`
- [ ] **Managing PR Lifecycles**
  - [ ] Updating out-of-date PRs: Merge base vs Rebase on base
  - [ ] Merge strategies in GitHub: Create merge commit, Squash and merge, Rebase and merge
  - [ ] GitHub CLI (`gh`) for PR creation, review, and merging from the terminal
