# 08 - GitHub Workflows

## 📋 Section Overview
Leverage the GitHub platform ecosystem: project management, repository automation, GitHub Actions CI/CD, environments, and static deployment.

## 🎯 Topic Checklist
- [ ] **Repository Architecture & Governance**
  - [ ] GitHub repository components: Issues, Discussions, Projects (Kanban), Wiki
  - [ ] Issue templates & Pull Request templates (`.github/ISSUE_TEMPLATE/`, `PULL_REQUEST_TEMPLATE.md`)
  - [ ] `SECURITY.md`, `LICENSE`, `CONTRIBUTING.md`, and `CODE_OF_CONDUCT.md`
- [ ] **Documentation & GitHub Flavored Markdown (GFM)**
  - [ ] Task lists, interactive checkboxes, tables, syntax highlighting
  - [ ] GitHub alerts (`[!NOTE]`, `[!TIP]`, `[!IMPORTANT]`, `[!WARNING]`, `[!CAUTION]`)
  - [ ] Embedding Mermaid architecture and sequence diagrams
  - [ ] Shield badges (status, license, version, build passing)
- [ ] **GitHub Actions (CI/CD)**
  - [ ] Core primitives: Workflows, Triggers (`on: push, pull_request`), Jobs, Steps, Runners
  - [ ] Writing a linting and test automation workflow (`.github/workflows/ci.yml`)
  - [ ] Action matrix builds across OS and language runtime versions
  - [ ] Caching dependencies (`actions/cache`) for accelerated builds
- [ ] **Secrets & Environment Management**
  - [ ] Repository Secrets vs Environment Secrets
  - [ ] Handling environment approvals and protection rules
  - [ ] OpenID Connect (OIDC) for cloud authentication (AWS/GCP/Azure) without long-lived keys
- [ ] **Releases & Deployment**
  - [ ] GitHub Releases with automated changelog generation
  - [ ] Publishing documentation via GitHub Pages
