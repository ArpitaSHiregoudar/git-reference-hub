# 13 - Git in DevOps

## 📋 Section Overview
How Git serves as the single source of truth for infrastructure, automated continuous deployment pipelines, security scanning, and compliance auditing.

## 🎯 Topic Checklist
- [ ] **GitOps Core Principles**
  - [ ] Declarative infrastructure stored entirely in version control
  - [ ] Automated state reconciliation (ArgoCD, Flux CD)
  - [ ] Pull-based vs push-based deployment architectures
- [ ] **Infrastructure as Code (IaC) in Git**
  - [ ] Structuring Terraform, OpenTofu, Kubernetes manifests in repositories
  - [ ] Monorepo vs Multi-repo patterns for microservices and infra
- [ ] **Security, Secret Detection & Compliance**
  - [ ] Pre-commit scanning for secrets (Gitleaks, TruffleHog)
  - [ ] GitHub Secret Scanning and Push Protection
  - [ ] Automated dependency vulnerability management (Dependabot, Renovate)
- [ ] **Cryptographic Verification & Audit Trails**
  - [ ] Signing commits and tags with GPG, SSH keys, or Sigstore
  - [ ] GitHub "Verified" commit badge enforcement via branch rulesets
  - [ ] Audit logs and regulatory compliance tracking
- [ ] **Branching Architectures Optimized for CI/CD**
  - [ ] Trunk-based delivery with canary and blue-green deployments
  - [ ] Environment promotion branches (`dev` ➔ `staging` ➔ `prod`)
  - [ ] Automated semantic release tagging (`semantic-release`, Release Please)
