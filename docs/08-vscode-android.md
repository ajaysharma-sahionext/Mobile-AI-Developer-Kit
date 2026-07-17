# 08 - VS Code Android

# Quick Summary

VS Code Android is the primary editor used throughout this guide.

It provides a familiar development experience for editing, searching, reviewing and managing projects, while Termux handles the terminal, package management and AI tools.

---

# Goal

After completing this chapter you will have:

* VS Code installed
* Storage access configured
* Workspace ready
* Recommended settings applied
* Projects connected to the Developer directory
* VS Code working together with Termux

---

# Why VS Code

VS Code is one of the most popular code editors.

Benefits include:

* Fast editing
* Multi-language support
* Syntax highlighting
* Search across projects
* File explorer
* Markdown support

It works well together with Termux.

---

# Why We Chose VS Code

Reasons:

* Familiar interface
* Excellent language support
* Lightweight enough for Android
* Large extension ecosystem (where supported)
* Great for React, Node.js and Python

---

# Alternatives

Other editors include:

* Acode
* Code Editor
* Squircle IDE

These are useful, but VS Code will be the primary editor throughout this guide.

---

# Installation

Install the latest stable VS Code Android application.

Always prefer the official release.

Avoid installing modified or unofficial builds.

---

# First Launch

Open VS Code.

Allow the initial setup to complete.

Grant the requested permissions when prompted.

---

# Storage Permission

Grant storage access.

VS Code should be able to access:

* Internal Storage
* Developer folder
* Projects folder

Without storage permission, projects cannot be opened correctly.

---

# Open Your Workspace

Navigate to:

```text
Developer/
Projects/
```

Open this folder as your primary workspace.

All future projects should be stored here.

---

# Recommended Theme

Choose any theme you prefer.

Recommended:

* Dark Theme
* High Contrast Dark

A dark theme reduces eye strain during long sessions.

---

# Recommended Font Size

Suggested values:

| Setting      | Value    |
| ------------ | -------- |
| Font Size    | 14–16    |
| Tab Size     | 2 or 4   |
| Word Wrap    | Enabled  |
| Line Numbers | Enabled  |
| Minimap      | Optional |

Adjust these according to your preference.

---

# Auto Save

Enable Auto Save.

Recommended delay:

* 1000 milliseconds

This reduces the chance of losing changes.

---

# File Associations

VS Code should correctly recognize:

* JavaScript
* TypeScript
* JSON
* Markdown
* Python
* YAML
* HTML
* CSS

No manual changes are normally required.

---

# Search

Learn the global search feature.

It allows searching across the entire project.

This becomes very useful in larger applications.

---

# Markdown Preview

Use VS Code for:

* Documentation
* README files
* Notes
* Prompt library

Markdown support is one of the strengths of VS Code.

---

# Project Structure

Every new project should follow:

```text
Projects/

React/

ReactNative/

Node/

Python/

Experiments/
```

Keeping projects organized improves navigation.

---

# Working with Termux

VS Code edits files.

Termux runs commands.

Typical workflow:

```text
Edit Code
      │
      ▼
Save File
      │
      ▼
Open Termux
      │
      ▼
Run Commands
      │
      ▼
View Results
      │
      ▼
Return to VS Code
```

This workflow will be used throughout the guide.

---

# Best Practices

* Keep one project open at a time.
* Close unused files.
* Save frequently.
* Keep the Explorer organized.
* Store projects inside the Developer folder.

---

# Common Mistakes

Avoid:

* Editing files directly from Downloads.
* Creating projects outside the Developer folder.
* Opening multiple large projects simultaneously.
* Ignoring storage permission requests.

---

# Troubleshooting

## Cannot Open Folder

Verify storage permission has been granted.

Restart VS Code if necessary.

---

## Files Missing

Refresh the Explorer.

Confirm the project exists inside the Developer directory.

---

## Slow Performance

Close unused tabs.

Close large folders that are not needed.

Restart the application if memory usage becomes high.

---

## Permission Errors

Check Android Settings.

Ensure VS Code has storage access.

---

# Optional Improvements

These enhancements can be added later:

* External Bluetooth keyboard
* External mouse
* Foldable phone stand
* External monitor (if supported)

These improve productivity but are not required.

---

# Verification Checklist

Confirm the following:

* ✅ VS Code installed
* ✅ Storage permission granted
* ✅ Developer folder accessible
* ✅ Projects folder opened
* ✅ Auto Save enabled
* ✅ Theme configured
* ✅ Basic editing working

If every item is complete, the editor is ready.

---

# Next Chapter

Continue with:

**09 - Git & GitHub**

The next chapter covers installing Git, configuring your identity, generating SSH keys, connecting GitHub, cloning repositories, and establishing the Git workflow that will be used throughout the remainder of this guide.
