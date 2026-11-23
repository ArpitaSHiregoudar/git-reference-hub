# 15 - Interview Preparation

## 📋 Section Overview
Comprehensive technical interview prep covering Git mental models, edge-case behavioral questions, scenario simulations, and quick-recall comparisons.

## 🎯 Topic Checklist
- [ ] **Foundational Architecture Questions**
  - [ ] How does Git store files internally compared to SVN or CVS?
  - [ ] What is an immutable Directed Acyclic Graph (DAG)?
  - [ ] Explain the structure and purpose of Blobs, Trees, Commits, and Annotated Tags.
  - [ ] What happens inside the `.git` folder when you run `git init`?
- [ ] **Command Comparison & Deep Nuance**
  - [ ] `git merge` vs `git rebase`: When should you prefer one over the other?
  - [ ] `git reset` vs `git revert`: Implications on shared vs private history
  - [ ] `git fetch` vs `git pull`: Why is `git pull` often considered dangerous without `--rebase`?
  - [ ] `git checkout` vs `git switch` vs `git restore`: Why did Git separate these concerns in 2.23+?
- [ ] **Troubleshooting & Scenario Challenges**
  - [ ] "You committed a 500MB video file 3 commits ago and can't push. How do you fix it?"
  - [ ] "A bug appeared in production that was not present two weeks ago. How do you find the offending commit in a repo with 5,000 commits?"
  - [ ] "Explain how `git reflog` differs from `git log`. Can `reflog` save uncommitted files?"
- [ ] **Enterprise Architecture & Governance**
  - [ ] Compare Git Flow vs GitHub Flow vs Trunk-Based Development for a team releasing to production multiple times per day.
  - [ ] How do you enforce mandatory code reviews and passing CI checks before merging?
- [ ] **Rapid Revision Cheat Sheet & Flashcard Matrix**
  - [ ] Quick-fire command syntax matrix
  - [ ] Common error messages and their immediate fixes
