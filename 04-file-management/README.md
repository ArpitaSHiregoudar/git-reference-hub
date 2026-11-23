# 04 - File Management

## 📋 Section Overview
Master how Git tracks file states, ignores build artifacts, handles binary dependencies with LFS, and manages cross-platform line endings.

## 🎯 Topic Checklist
- [ ] **The Git File Lifecycle**
  - [ ] Untracked ➔ Staged ➔ Unmodified ➔ Modified state loop
  - [ ] Detecting ignored vs untracked states
- [ ] **Mastering `.gitignore`**
  - [ ] Pattern syntax: globbing, wildcards, directory exclusion, and negation (`!`)
  - [ ] Project-level `.gitignore` vs Global `.gitignore` (`core.excludesFile`)
  - [ ] Untracking files already committed to history (`git rm --cached`)
  - [ ] Debugging ignore rules (`git check-ignore -v <path>`)
- [ ] **Cross-Platform Consistency (`.gitattributes`)**
  - [ ] Normalizing line endings across Windows (CRLF) and Linux/macOS (LF)
  - [ ] Declaring binary files explicitly (`*.png binary`, `*.pdf -text`)
  - [ ] Custom merge drivers and diff drivers
- [ ] **Handling Large Assets with Git LFS (Large File Storage)**
  - [ ] The problem with large binary files in standard Git histories
  - [ ] Installing and initializing Git LFS (`git lfs install`)
  - [ ] Tracking large file types with `.gitattributes` (`git lfs track "*.psd"`)
  - [ ] Pushing, pulling, and cloning LFS-enabled repositories
- [ ] **Empty Directories & Conventions**
  - [ ] Why Git does not track empty folders
  - [ ] Industry standard `.gitkeep` pattern and `.gitignore` inside empty folders
