# CommitCraft 🛠️
> **The Definitive Git & GitHub Engineering Reference Hub**  
> *Repository: `git-reference-hub`*

---

## 🎯 Purpose of CommitCraft

**CommitCraft** is an end-to-end, production-grade knowledge architecture designed to take developers from fundamental source control concepts to enterprise-level Git mastery and DevOps integration.

Version control is not merely a utility for saving code—it is the operational backbone of modern collaborative software engineering. CommitCraft addresses common industry pain points:
- Moving beyond rote command memorization to internalizing **Git's underlying mental model** (directed acyclic graphs, content-addressable storage, snapshot architectures).
- Bridging the gap between **local Git operations** and **cloud-scale GitHub collaboration workflows**.
- Empowering engineers to execute fearless recovery maneuvers when complex merge conflicts, detached HEADs, or history corruptions occur.
- Preparing engineers for technical code reviews, enterprise branching governance, CI/CD integration, and high-stakes technical interviews.

---

## 🧭 Repository Architecture

The repository is modularized into 15 progressive sections:

| # | Section | Focus Area | Complexity |
|---|---|---|---|
| **01** | [`01-git-fundamentals/`](./01-git-fundamentals/) | Core concepts, VCS vs DVCS, Git internal architecture, object model | Foundation |
| **02** | [`02-git-configuration/`](./02-git-configuration/) | Scopes, identities, credential helpers, SSH/GPG, conditional includes | Foundation |
| **03** | [`03-essential-commands/`](./03-essential-commands/) | Staging patterns, commits, diffing, log filtering, inspection | Core Practice |
| **04** | [`04-file-management/`](./04-file-management/) | Lifecycle states, `.gitignore`, Git LFS, `.gitattributes`, line endings | Core Practice |
| **05** | [`05-branching-strategies/`](./05-branching-strategies/) | Branch pointers, Git Flow, GitHub Flow, Trunk-Based Development | Core Practice |
| **06** | [`06-merging-and-conflicts/`](./06-merging-and-conflicts/) | Fast-forward, 3-way, squash, conflict resolution, `git rerere` | Intermediate |
| **07** | [`07-remote-repositories/`](./07-remote-repositories/) | Tracking branches, fetch vs pull, push flags, pruning, multiple remotes | Intermediate |
| **08** | [`08-github-workflows/`](./08-github-workflows/) | Issues, Projects, GitHub Actions CI/CD, Secrets, Pages, Releases | Intermediate |
| **09** | [`09-pull-requests-and-reviews/`](./09-pull-requests-and-reviews/) | PR anatomy, code review etiquette, branch protection, rulesets | Collaboration |
| **10** | [`10-git-undo-magic/`](./10-git-undo-magic/) | `restore`, `reset` modes, `revert`, `stash`, and the life-saving `reflog` | Advanced |
| **11** | [`11-advanced-git/`](./11-advanced-git/) | Interactive rebase, `bisect`, cherry-pick, submodules, worktrees, hooks | Advanced |
| **12** | [`12-collaboration-and-teamwork/`](./12-collaboration-and-teamwork/) | Forking model, upstream sync, conventional commits, `CODEOWNERS` | Enterprise |
| **13** | [`13-git-in-devops/`](./13-git-in-devops/) | GitOps (ArgoCD/Flux), secret scanning, pipeline branching, signed tags | DevOps |
| **14** | [`14-real-world-scenarios/`](./14-real-world-scenarios/) | Production triage playbooks: accidental commits, leaked secrets, merge panics | Applied Triage |
| **15** | [`15-interview-preparation/`](./15-interview-preparation/) | High-yield conceptual Q&A, scenario challenges, architecture cheat sheets | Career & Assessment |

---

## 🗺️ Recommended Learning Sequence

CommitCraft supports three personalized pathways depending on your experience level:

```
[Phase 1: Foundations]
01-git-fundamentals ➔ 02-git-configuration ➔ 03-essential-commands ➔ 04-file-management
                                │
                                ▼
[Phase 2: Branching & Collaboration]
05-branching-strategies ➔ 06-merging-and-conflicts ➔ 07-remote-repositories ➔ 08-github-workflows ➔ 09-pull-requests-and-reviews
                                │
                                ▼
[Phase 3: Power User & Disaster Recovery]
10-git-undo-magic ➔ 11-advanced-git ➔ 12-collaboration-and-teamwork
                                │
                                ▼
[Phase 4: Enterprise & Professional Readiness]
13-git-in-devops ➔ 14-real-world-scenarios ➔ 15-interview-preparation
```

1. **The Fast-Track (Beginner to Daily Committer):**  
   Modules `01` ➔ `02` ➔ `03` ➔ `05` ➔ `07` ➔ `09`
2. **The Senior Engineer / Triage Track (Mastering Complexity):**  
   Modules `06` ➔ `10` ➔ `11` ➔ `14`
3. **The DevOps & Tech Lead Track (Governance & Infrastructure):**  
   Modules `08` ➔ `12` ➔ `13` ➔ `15`

---

## 📌 Status

- [x] Workspace directory scaffolding complete (15 modules)
- [x] Architectural design & root reference documented
- [x] Topic checklists established for all 15 modules
- [ ] Detailed notes, visual diagrams, and code playbooks *(Pending User Approval)*
