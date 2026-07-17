# 09 - Git & GitHub

# Quick Summary

Git is the version control system used throughout this guide.

GitHub provides remote repository hosting, collaboration, backup and version history.

After completing this chapter, you'll have a fully functional Git workflow on Android.

---

# Goal

After completing this chapter you will have:

* Git installed
* Git configured
* GitHub account ready
* SSH authentication configured
* Repository cloning working
* Push and Pull working
* Professional Git workflow ready

---

# Why Git

Git allows you to:

* Track changes
* Restore previous versions
* Work with branches
* Collaborate with others
* Backup projects

Every project should use Git from day one.

---

# Why GitHub

GitHub provides:

* Remote repositories
* Unlimited public repositories
* Private repositories
* Collaboration
* Pull Requests
* Issues
* Releases
* Project backup

---

# Install Git

Git should already be installed from the previous chapter.

Verify installation:

```bash
git --version
```

If Git is missing:

```bash
pkg install git
```

---

# Configure Git

Configure your identity.

```bash
git config --global user.name "Your Name"

git config --global user.email "your@email.com"
```

Verify:

```bash
git config --list
```

---

# Recommended Git Settings

```bash
git config --global init.defaultBranch main

git config --global pull.rebase false

git config --global core.editor nano
```

These settings provide a simple and beginner-friendly workflow.

---

# Generate SSH Key

Create a new SSH key.

```bash
ssh-keygen -t ed25519 -C "your@email.com"
```

Press Enter for all default options.

---

# Verify SSH Keys

List generated keys:

```bash
ls ~/.ssh
```

You should see files similar to:

```text
id_ed25519
id_ed25519.pub
```

---

# Copy Public Key

Display the public key:

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the entire output.

---

# Add SSH Key to GitHub

Open GitHub.

Navigate to:

Settings

↓

SSH and GPG Keys

↓

New SSH Key

Paste your public key and save it.

---

# Test SSH Connection

Run:

```bash
ssh -T git@github.com
```

The first connection will ask for confirmation.

Type:

```text
yes
```

If successful, GitHub will display a welcome message.

---

# Clone Repository

Clone an existing repository.

```bash
git clone git@github.com:username/repository.git
```

The project will be downloaded to the current directory.

---

# Create New Repository

Inside your project:

```bash
git init
```

---

# Check Status

```bash
git status
```

Always check status before committing.

---

# Add Files

Add all files.

```bash
git add .
```

---

# Commit Changes

```bash
git commit -m "Initial commit"
```

Use short and meaningful commit messages.

---

# Connect Remote Repository

```bash
git remote add origin git@github.com:username/repository.git
```

Verify:

```bash
git remote -v
```

---

# Push Changes

First push:

```bash
git push -u origin main
```

Later pushes:

```bash
git push
```

---

# Pull Changes

```bash
git pull
```

Always pull before starting new work.

---

# Branch Workflow

Recommended branches:

```text
main
development
feature/login
feature/profile
feature/chat
hotfix
release
```

---

# Create Branch

```bash
git checkout -b feature/login
```

---

# Switch Branch

```bash
git checkout main
```

---

# Merge Branch

```bash
git merge feature/login
```

Merge only after testing.

---

# Git Ignore

Every project should include a `.gitignore` file.

Examples:

* node_modules
* .expo
* build
* dist
* .env
* .DS_Store

Templates will be provided later in this guide.

---

# Useful Commands

```bash
git status

git log

git diff

git branch

git branch -a

git remote -v

git stash

git stash pop

git fetch

git pull

git push
```

---

# Recommended Workflow

```text
Create Project

↓

git init

↓

Create Repository

↓

git add .

↓

git commit

↓

git push

↓

Create Feature Branch

↓

Develop

↓

Commit

↓

Push

↓

Merge
```

---

# Best Practices

* Commit frequently.
* Use meaningful commit messages.
* Keep commits focused.
* Pull before pushing.
* Never commit passwords or API keys.
* Use feature branches.
* Push regularly.

---

# Common Mistakes

Avoid:

* Working directly on main
* Committing large generated files
* Committing node_modules
* Committing .env files
* Force pushing without understanding the impact

---

# Troubleshooting

## Permission Denied (publickey)

Verify:

* SSH key exists
* Public key added to GitHub
* SSH connection tested

---

## Authentication Failed

Check:

```bash
ssh -T git@github.com
```

---

## Repository Not Found

Verify:

* Repository exists
* URL is correct
* You have access

---

## Merge Conflicts

Review conflicting files carefully.

Resolve conflicts manually before committing.

---

# Verification Checklist

Confirm:

* ✅ Git installed
* ✅ Git configured
* ✅ GitHub account available
* ✅ SSH key generated
* ✅ SSH key added to GitHub
* ✅ SSH connection successful
* ✅ Repository cloned
* ✅ Push working
* ✅ Pull working
* ✅ Branch creation working

If every item is complete, your Git environment is fully configured.

---

# Optional Improvements

These enhancements will be added later:

* Git aliases
* Custom .gitconfig
* Global .gitignore
* Automatic backup scripts
* Git automation
* Repository templates
* GitHub Actions
* Release automation

---

# Next Chapter

Continue with:

**10 - Node.js & Python**

In the next chapter we'll install and configure the complete JavaScript and Python development environment, including npm, package management, virtual environments, useful developer tools, and verification steps required before installing Ollama.
