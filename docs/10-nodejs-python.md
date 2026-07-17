# 10 - Node.js & Python

# Quick Summary

Node.js and Python are the primary programming runtimes used throughout this guide.

Node.js powers JavaScript, TypeScript, React, React Native and Expo development, while Python is used for automation, scripting, AI utilities and development tools.

---

# Goal

After completing this chapter you will have:

* Node.js installed
* npm installed
* Python installed
* pip installed
* Development environment verified
* Basic package management knowledge

---

# Prerequisites

Complete the following chapters first:

* Android Preparation
* Termux
* Git & GitHub

---

# Why Node.js

Node.js is required for:

* React
* React Native
* Expo
* JavaScript
* TypeScript
* Build tools
* Package management

Almost every JavaScript project depends on Node.js.

---

# Why Python

Python is used for:

* Automation
* Utility scripts
* AI tools
* Data processing
* Development helpers

Several later chapters depend on Python.

---

# Verify Existing Installation

Run:

```bash
node --version

npm --version

python --version

pip --version
```

If every command returns a version number, continue.

Otherwise install the missing packages.

---

# Install Node.js

```bash
pkg install nodejs
```

Verify:

```bash
node --version

npm --version
```

---

# Install Python

```bash
pkg install python
```

Verify:

```bash
python --version

pip --version
```

---

# Update npm

Keeping npm updated improves compatibility.

```bash
npm install -g npm
```

Verify:

```bash
npm --version
```

---

# Upgrade pip

Upgrade pip to the latest available version.

```bash
python -m pip install --upgrade pip
```

Verify:

```bash
pip --version
```

---

# Install Common Global npm Packages

Install commonly used development tools.

```bash
npm install -g \
typescript \
eslint \
prettier \
npm-check-updates
```

These packages are useful for most JavaScript projects.

---

# Install Common Python Packages

Install useful Python tools.

```bash
pip install \
virtualenv \
black \
isort \
flake8
```

These tools help with formatting and development.

---

# Verify Global Packages

Node.js:

```bash
npm list -g --depth=0
```

Python:

```bash
pip list
```

Review the installed packages.

---

# Create a Test Project

Create a temporary directory.

```bash
mkdir ~/Developer/TestProject

cd ~/Developer/TestProject
```

---

# Test Node.js

Create a file named:

```text
test.js
```

Contents:

```javascript
console.log("Node.js is working!");
```

Run:

```bash
node test.js
```

Expected output:

```text
Node.js is working!
```

---

# Test Python

Create:

```text
test.py
```

Contents:

```python
print("Python is working!")
```

Run:

```bash
python test.py
```

Expected output:

```text
Python is working!
```

---

# Recommended Project Layout

```text
Projects/

React/

ReactNative/

Node/

Python/
```

Store each project inside its appropriate folder.

---

# Package Management

Node.js

```bash
npm install

npm update

npm uninstall
```

Python

```bash
pip install

pip uninstall

pip list
```

Only install packages that are actually needed.

---

# Best Practices

* Keep Node.js updated.
* Keep Python updated.
* Remove unused packages.
* Use project-specific dependencies.
* Keep global packages to a minimum.

---

# Common Mistakes

Avoid:

* Installing unnecessary global npm packages.
* Mixing project dependencies with global tools.
* Ignoring package updates.
* Installing duplicate packages.

---

# Troubleshooting

## npm Command Not Found

Reinstall Node.js.

```bash
pkg install nodejs
```

---

## pip Command Not Found

Reinstall Python.

```bash
pkg install python
```

---

## Package Installation Failed

Update packages first.

```bash
pkg update

pkg upgrade
```

Retry the installation.

---

## Permission Errors

Avoid using sudo.

Termux does not require it.

---

# Verification Checklist

Confirm:

* ✅ Node.js installed
* ✅ npm installed
* ✅ Python installed
* ✅ pip installed
* ✅ Test JavaScript executed
* ✅ Test Python script executed
* ✅ Global packages installed

If all checks pass, your development runtime is ready.

---

# Best Practices

* Update runtimes regularly.
* Keep global packages minimal.
* Create one project per folder.
* Use version control for every project.
* Remove test files after verification.

---

# Developer Notes

Node.js and Python are installed early because almost every modern development tool depends on one of them.

Later chapters—including Expo, React Native, Ollama utilities and automation scripts—will build on this foundation.

---

# References

* Official Node.js Documentation
* Official npm Documentation
* Official Python Documentation
* Official pip Documentation

---

# Next Chapter

Continue with:

**11 - Ollama**

The next chapter covers installing Ollama on Android, understanding how local AI works, selecting the right models for an 8GB device, managing storage, optimizing performance and preparing the AI engine that powers the remainder of this guide.
