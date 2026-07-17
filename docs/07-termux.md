# 07 - Termux

# Quick Summary

Termux is the foundation of the entire Mobile AI Developer Kit.

It provides a Linux environment on Android where we will install Git, Node.js, Python, Ollama, development tools, automation scripts and AI workflows.

Everything in the following chapters depends on a properly configured Termux installation.

---

# Goal

After completing this chapter you will have:

* Latest Termux installed
* Storage access configured
* Package repositories updated
* Essential Linux packages installed
* Shell ready for development
* Development workspace prepared

---

# Why Termux

Termux provides a lightweight Linux environment without requiring root access.

It allows Android devices to behave much more like a traditional development machine.

---

# Why F-Droid Version

Always install the F-Droid version.

Reasons:

* Latest updates
* Better package compatibility
* Officially maintained
* Recommended by the Termux project

Avoid the outdated Google Play version.

---

# Installation

1. Install F-Droid.
2. Open F-Droid.
3. Search for **Termux**.
4. Install the latest stable release.
5. Launch the application.

Allow a few moments for the first launch to complete.

---

# First Launch

When Termux opens for the first time:

* Wait for initialization.
* Do not interrupt the process.
* Keep the screen awake until initialization finishes.

---

# Grant Storage Permission

Run:

```bash
termux-setup-storage
```

Grant storage permission when Android asks.

This creates access to shared device storage.

---

# Update Packages

Always update the package repository before installing anything.

```bash
pkg update
pkg upgrade -y
```

Repeat this regularly to keep packages current.

---

# Install Essential Packages

Install the base development tools.

```bash
pkg install -y \
git \
curl \
wget \
nano \
vim \
zip \
unzip \
tar \
tree \
openssh \
ripgrep \
fd \
which \
htop \
jq \
python \
python-pip \
nodejs \
clang \
make \
cmake
```

These packages are sufficient for most development tasks in this guide.

---

# Verify Installation

Check the installed versions:

```bash
git --version
python --version
pip --version
node --version
npm --version
```

All commands should return a version number without errors.

---

# Recommended Workspace

Create the development directory:

```bash
mkdir -p ~/Developer
cd ~/Developer
```

This becomes the primary workspace inside Termux.

---

# Basic Linux Commands

Useful commands:

```bash
pwd
ls
cd
mkdir
rm
cp
mv
cat
clear
history
```

These commands will be used throughout the guide.

---

# Shell Tips

Useful shortcuts:

| Shortcut   | Action               |
| ---------- | -------------------- |
| Ctrl + C   | Stop current process |
| Ctrl + D   | Exit shell           |
| Arrow Up   | Previous command     |
| Arrow Down | Next command         |
| Tab        | Auto-complete        |

Learning these shortcuts improves productivity.

---

# Keep Packages Updated

Run periodically:

```bash
pkg update
pkg upgrade -y
```

This helps avoid compatibility issues.

---

# Best Practices

* Use Termux for all terminal commands.
* Keep the environment clean.
* Install only required packages.
* Update packages regularly.
* Restart Termux after major updates if needed.

---

# Common Mistakes

Avoid:

* Using the Play Store version of Termux.
* Skipping `termux-setup-storage`.
* Installing unnecessary packages.
* Running commands as root.
* Copying commands without reading them.

---

# Troubleshooting

## Storage Not Accessible

Run:

```bash
termux-setup-storage
```

again and confirm the permission dialog.

---

## Package Installation Fails

Update package lists:

```bash
pkg update
pkg upgrade
```

Then retry the installation.

---

## Command Not Found

Verify the package is installed correctly.

Example:

```bash
pkg install git
```

---

## Permission Denied

Restart Termux after granting permissions.

If needed, check Android app permissions manually.

---

# Optional Improvements

These can be configured later:

* Zsh shell
* Starship prompt
* SSH configuration
* Git aliases
* Custom shell aliases
* Development scripts
* Automatic backups

Keeping the initial setup simple is recommended.

---

# Verification Checklist

Confirm the following:

* ✅ Latest Termux installed
* ✅ Storage permission granted
* ✅ Packages updated
* ✅ Essential packages installed
* ✅ Git working
* ✅ Node.js working
* ✅ Python working
* ✅ Developer workspace created

If every item is complete, your Linux development environment is ready.

---

# Next Chapter

Continue with:

**08 - VS Code Android**

The next chapter covers installing, configuring and optimizing VS Code for Android, including workspace management, file access, recommended settings and the workflow we'll use alongside Termux.
