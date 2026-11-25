# 03. SSH & Authentication

---

## Why Do You Need Authentication?

When you `git push` or `git pull` from a remote repository (like GitHub), the server needs to verify **who you are**. There are two main ways to authenticate:

| Method | How It Works | Best For |
|---|---|---|
| **SSH Key** | A cryptographic key pair (public + private) stored on your machine. No password needed after setup. | Daily development — push/pull without entering credentials. |
| **Personal Access Token (PAT)** | A generated token string used as a password substitute over HTTPS. | Scripts, CI/CD, or when SSH is not available. |

---

## Option 1: SSH Key Setup (Recommended)

### Step 1 — Check for existing keys

```bash
ls -al ~/.ssh
# Look for files like id_ed25519 and id_ed25519.pub
```

If they already exist, you can skip to Step 3.

### Step 2 — Generate a new SSH key

```bash
ssh-keygen -t ed25519 -C "your.email@example.com"
```

- `-t ed25519` — The key type. Ed25519 is modern and secure (preferred over older RSA).
- `-C "email"` — A label to identify the key.

When prompted:
- **File location:** Press Enter to accept the default (`~/.ssh/id_ed25519`).
- **Passphrase:** Optional but recommended. Adds an extra layer of security.

This creates two files:

| File | What It Is | Share It? |
|---|---|---|
| `id_ed25519` | Your **private** key. | ❌ **Never share this.** |
| `id_ed25519.pub` | Your **public** key. | ✅ This goes to GitHub. |

### Step 3 — Add the key to the SSH agent

```bash
# Start the SSH agent
eval "$(ssh-agent -s)"

# Add your private key
ssh-add ~/.ssh/id_ed25519
```

**On Windows (PowerShell):**

```powershell
# Start the agent service if not running
Get-Service ssh-agent | Set-Service -StartupType Automatic
Start-Service ssh-agent

# Add the key
ssh-add $env:USERPROFILE\.ssh\id_ed25519
```

### Step 4 — Add the public key to GitHub

1. Copy your public key:

```bash
cat ~/.ssh/id_ed25519.pub
# Copy the entire output
```

2. Go to **GitHub → Settings → SSH and GPG Keys → New SSH Key**.
3. Paste the public key and give it a title (e.g., "My Laptop").
4. Click **Add SSH Key**.

### Step 5 — Test the connection

```bash
ssh -T git@github.com
```

Expected output:

```
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

### Step 6 — Use SSH URLs for repos

When cloning or adding remotes, use the SSH URL format:

```bash
# SSH URL (use this)
git clone git@github.com:username/repo.git

# HTTPS URL (alternative)
git clone https://github.com/username/repo.git
```

---

## Option 2: Personal Access Tokens (PATs)

PATs are used when authenticating over **HTTPS** instead of SSH.

### When to use PATs
- Automated scripts and CI/CD pipelines.
- Environments where SSH is blocked.
- Temporary or limited access needs.

### How to create one

1. Go to **GitHub → Settings → Developer Settings → Personal Access Tokens → Tokens (classic)**.
2. Click **Generate new token**.
3. Select scopes (permissions) — at minimum, select `repo` for full repository access.
4. Copy the token immediately (you won't see it again).

### Using it

When Git asks for your password over HTTPS, paste the **token** instead of your GitHub password.

---

## Option 3: Git Credential Manager (GCM)

If you use HTTPS frequently, **Git Credential Manager** saves your credentials securely so you don't have to enter them every time.

It comes **pre-installed with Git for Windows**. On Mac/Linux:

```bash
# Check if installed
git credential-manager --version
```

GCM automatically stores your tokens in the OS keychain (Windows Credential Store / macOS Keychain / Linux Secret Service).

---

## Quick Comparison

| Feature | SSH Key | Personal Access Token | Credential Manager |
|---|---|---|---|
| **Protocol** | SSH (`git@github.com:...`) | HTTPS (`https://github.com/...`) | HTTPS (auto-cached) |
| **Setup** | Generate key pair, add public key to GitHub | Generate token on GitHub | Usually pre-installed |
| **Enter credentials?** | No (after setup) | Yes (first time per repo) | No (after first time) |
| **Best for** | Daily development | Scripts & CI/CD | Casual HTTPS users |

---

## 🎯 Interview Ready

**Q: What is the difference between SSH and HTTPS authentication in Git?**
> SSH uses a cryptographic key pair — the private key stays on your machine and the public key is registered with GitHub. After setup, no password is needed. HTTPS uses a username and token (or password) for each connection, though credentials can be cached using Git Credential Manager.

**Q: Why is Ed25519 preferred over RSA for SSH keys?**
> Ed25519 keys are shorter, faster to generate, and provide equivalent or better security than RSA keys. They are the modern recommended standard.

**Q: What is a Personal Access Token and when would you use one?**
> A PAT is a token generated on GitHub that acts as a password substitute for HTTPS authentication. It is commonly used in automated scripts, CI/CD pipelines, or environments where SSH is not available.

---

> **Next →** [04-multi-profile-setup.md](./04-multi-profile-setup.md) — Set up separate Git identities for personal and work projects.
