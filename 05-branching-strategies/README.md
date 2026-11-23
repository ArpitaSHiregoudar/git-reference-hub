# 05 - Branching Strategies

## 📋 Section Overview
Dive into how Git implements branches as lightweight pointers, branch lifecycle management, and enterprise-grade branching workflows.

## 🎯 Topic Checklist
- [ ] **Branch Mechanics Under the Hood**
  - [ ] What is a branch? (A 41-byte pointer file in `.git/refs/heads/`)
  - [ ] The `HEAD` pointer: How Git knows what branch you are on
  - [ ] Detached `HEAD` state: Causes, mechanics, and recovery
- [ ] **Branch Operations**
  - [ ] Creating branches (`git branch <name>`)
  - [ ] Modern branch switching: `git switch` vs legacy `git checkout`
  - [ ] Creating and switching in one command (`git switch -c <name>`)
  - [ ] Renaming branches locally and remotely (`git branch -m`)
  - [ ] Deleting merged vs unmerged branches (`git branch -d` vs `git branch -D`)
  - [ ] Listing local, remote, and tracking branches (`git branch -vv -a`)
- [ ] **Branch Comparison & Inspection**
  - [ ] Double-dot vs Triple-dot syntax (`git diff main..feature` vs `git diff main...feature`)
  - [ ] Finding branches containing specific commits (`git branch --contains`)
- [ ] **Industry Branching Models & Governance**
  - [ ] **Git Flow**: Roles of `main`, `develop`, `feature/*`, `release/*`, `hotfix/*`
  - [ ] **GitHub Flow**: Minimalist, deployment-driven, main-branch centric
  - [ ] **GitLab Flow**: Environment branches (`staging`, `production`) and release branches
  - [ ] **Trunk-Based Development**: Short-lived branches, feature flags, continuous delivery
  - [ ] Choosing the right model for your team size and deployment cadence
