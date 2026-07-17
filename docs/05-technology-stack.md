# 05 - Technology Stack

# Quick Summary

Before installing any software, it is important to understand the technology stack used throughout this guide.

Every tool has been selected for stability, long-term support, community adoption and compatibility with Android.

---

# Goal

This chapter introduces every major technology that will be used throughout the project.

By the end of this chapter you will understand why each tool has been selected before installing it.

---

# Design Principles

Every tool included in this guide follows these principles:

* Free when possible
* Open Source preferred
* Beginner friendly
* Stable
* Well documented
* Long-term maintainable
* Android compatible

---

# Core Operating Environment

The development environment consists of:

* Android
* Linux (Termux)
* Local AI
* Git
* VS Code
* Open Source Tools

---

# Android

Android provides the base operating system.

It manages hardware, storage, networking, permissions and application lifecycle.

No root access is required.

---

# Termux

Termux provides a Linux userspace on Android.

It allows installation of developer tools including:

* Git
* Python
* Node.js
* SSH
* Build tools

Nearly every command in this guide will be executed inside Termux.

---

# Git

Git manages source code.

It provides:

* Version history
* Branch management
* Collaboration
* Backup

Every project should be stored inside a Git repository.

---

# GitHub

GitHub is recommended for:

* Remote repositories
* Backup
* Collaboration
* Issue tracking
* Releases

Alternative Git providers may also be used.

---

# Node.js

Node.js is required for:

* React
* React Native
* Expo
* JavaScript tools
* TypeScript
* Package management

It will be installed inside Termux.

---

# Python

Python is used for:

* Automation
* Utilities
* AI tools
* Development scripts

Several later chapters depend on Python.

---

# Ollama

Ollama provides a simple interface for running local AI models.

It allows AI inference directly on supported hardware.

Different models can be downloaded depending on available memory.

---

# VS Code

VS Code serves as the primary code editor.

It will be used for:

* Editing
* Searching
* Reviewing
* Project navigation

Terminal operations will continue inside Termux.

---

# AI Models

Different models are suitable for different tasks.

Examples include:

* Coding
* Documentation
* Refactoring
* Debugging
* Reasoning

Model selection will be covered later.

---

# Markdown

Markdown is used for:

* Documentation
* Notes
* AI prompts
* Project memory

This entire repository is written using Markdown.

---

# Bash

Shell scripts automate repetitive tasks.

Examples include:

* Updating packages
* Starting development tools
* Cleaning temporary files
* Project setup

Automation chapters will build upon Bash scripts.

---

# SSH

SSH enables secure communication with Git providers and remote systems.

It is strongly recommended for GitHub authentication.

---

# Why This Stack

This stack was selected because it is:

* Lightweight
* Free
* Well supported
* Portable
* Reliable
* Beginner friendly

Every component works together without requiring root access.

---

# Technologies Not Included

This guide intentionally does not require:

* Root access
* Custom ROMs
* Linux distributions
* Virtual machines
* Paid AI subscriptions
* Proprietary development environments

Optional integrations may be covered later.

---

# Technology Flow

```text
Android
      │
      ▼
Termux
      │
      ├── Git
      ├── Python
      ├── Node.js
      ├── Bash
      └── SSH
             │
             ▼
          Ollama
             │
             ▼
         Local AI Models
             │
             ▼
        VS Code Android
             │
             ▼
       Application Development
```

---

# Verification

You should now understand the purpose of each major component.

No software installation is required in this chapter.

---

# Best Practices

* Use open-source tools whenever possible.
* Keep the stack simple.
* Avoid installing unnecessary software.
* Learn one tool before adding another.
* Update tools regularly.

---

# Next Chapter

Continue with:

**06 - Required Applications**

The next chapter introduces every application that must be installed before building the development environment.
