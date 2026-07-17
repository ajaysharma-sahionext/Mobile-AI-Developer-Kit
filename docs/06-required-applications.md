# 06 - Required Applications

# Quick Summary

This chapter lists every application required for the Mobile AI Developer Kit.

Do not install additional tools unless they are specifically recommended later in this guide.

A smaller and cleaner setup is easier to maintain.

---

# Goal

After completing this chapter you will have every required application installed before starting the development environment setup.

---

# Installation Order

Always install applications in the following order:

1. F-Droid
2. Termux
3. VS Code
4. Git (inside Termux)
5. Node.js
6. Python
7. Ollama
8. GitHub Authentication
9. AI Models

Do not skip steps.

---

# Required Applications

| Application     | Required | Purpose                          |
| --------------- | -------- | -------------------------------- |
| F-Droid         | ✅        | Install trusted open-source apps |
| Termux          | ✅        | Linux development environment    |
| VS Code Android | ✅        | Code editor                      |
| Git             | ✅        | Version control                  |
| Node.js         | ✅        | JavaScript runtime               |
| Python          | ✅        | Automation and scripting         |
| Ollama          | ✅        | Local AI runtime                 |

---

# Recommended Applications

These applications improve productivity but are not required.

| Application    | Purpose                  |
| -------------- | ------------------------ |
| Acode          | Lightweight code editor  |
| ZArchiver      | Archive management       |
| Material Files | File manager             |
| GitHub Mobile  | Repository notifications |
| KeePassDX      | Password manager         |
| LocalSend      | Offline file transfer    |

---

# Why F-Droid

F-Droid provides trusted open-source Android applications.

The latest Termux releases are distributed through F-Droid instead of the Google Play Store.

Always prefer the F-Droid version.

---

# Why Termux

Termux provides a Linux userspace on Android.

It becomes the primary terminal used throughout this guide.

Almost every development command will run inside Termux.

---

# Why VS Code

VS Code provides:

* Modern code editing
* Search
* Syntax highlighting
* Multi-language support

It works well together with Termux.

---

# Why Git

Git provides:

* Version history
* Branch management
* Collaboration
* Backup

Every project should use Git.

---

# Why Node.js

Node.js is required for:

* React
* React Native
* Expo
* JavaScript tooling
* TypeScript

---

# Why Python

Python is used for:

* Automation
* Utilities
* Development scripts
* AI helper tools

---

# Why Ollama

Ollama allows supported AI models to run locally.

It becomes the AI engine used throughout this project.

Model installation will be covered later.

---

# Applications Not Recommended

The following are intentionally excluded from the base setup:

* Root-only tools
* Duplicate terminal applications
* Multiple code editors
* Multiple package managers
* Experimental AI runtimes

Keeping the environment simple improves reliability.

---

# Installation Checklist

Confirm the following:

* F-Droid installed
* Termux installed
* VS Code installed

Git, Node.js, Python and Ollama will be installed in the next chapters.

---

# Verification

At this point your Android device should contain:

* F-Droid
* Termux
* VS Code

Nothing else needs to be configured yet.

---

# Troubleshooting

## Cannot install from F-Droid

Ensure installation from trusted sources is allowed according to your Android version.

---

## Multiple Termux Versions Installed

Remove duplicate installations.

Only use the F-Droid version.

---

## VS Code Cannot Access Files

Grant storage permission when prompted.

---

# Best Practices

* Install only required applications.
* Avoid duplicate developer tools.
* Keep applications updated.
* Download software only from official sources.
* Do not install unnecessary plugins yet.

---

# Optional Improvements

The following tools may be added later:

* GitHub Mobile
* LocalSend
* SSH client utilities
* Markdown preview tools

These are not required for the base environment.

---

# Next Chapter

Continue with:

**07 - Installing F-Droid**

The next chapter installs F-Droid correctly and explains why it is the preferred source for open-source Android development applications.
