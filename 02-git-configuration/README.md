# 02 - Git Configuration

## 📋 Section Overview
Understand how to configure Git across environments, manage credentials, customize developer ergonomics, and isolate personal vs work identities.

## 🎯 Topic Checklist
- [ ] **Configuration Scopes & Precedence**
  - [ ] System level (`/etc/gitconfig` or Windows equivalent)
  - [ ] Global level (`~/.gitconfig` or `%USERPROFILE%\.gitconfig`)
  - [ ] Local level (`.git/config` inside repository)
  - [ ] Worktree level (`.git/config.worktree`)
  - [ ] Inspecting effective configuration (`git config --list --show-origin`)
- [ ] **Essential Identity & Core Settings**
  - [ ] User identity: `user.name` and `user.email`
  - [ ] Default initial branch name: `init.defaultBranch main`
  - [ ] Default editor configuration (VS Code, Nano, Vim)
  - [ ] Line ending management (`core.autocrlf` for Windows vs macOS/Linux)
  - [ ] Safe line conversions (`core.safecrlf`)
- [ ] **Developer Ergonomics & Productivity**
  - [ ] Global Git aliases for high-frequency commands
  - [ ] Color output & UI personalization
  - [ ] Pager configurations (`delta`, `less`)
- [ ] **Authentication & Security Setup**
  - [ ] SSH Key generation (Ed25519 vs RSA), agent caching, and GitHub association
  - [ ] Personal Access Tokens (PATs) and fine-grained permissions
  - [ ] Git Credential Manager (GCM) setup and credential caching
- [ ] **Multi-Profile Git Configuration**
  - [ ] Conditional configuration with `includeIf` (Personal vs Work repositories)
  - [ ] Directory-based email and GPG signing segregation
