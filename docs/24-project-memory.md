# 24 - Project Memory

# Quick Summary

One of the biggest limitations of AI is the lack of long-term project understanding.

Project Memory solves this problem by storing important project information in a structured format that can be reused across development sessions.

Instead of repeatedly explaining your project to AI, maintain a single source of truth inside your project.

---

# Goal

After completing this chapter you will:

* Understand Project Memory
* Build a reusable AI knowledge base
* Reduce repetitive prompts
* Improve AI consistency
* Keep project information organized
* Create a Cursor-like project context

---

# What is Project Memory?

Project Memory is a collection of files that describe your project.

These files help AI understand:

* What the project does
* How it is organized
* Which technologies are used
* Which coding standards should be followed
* Important architectural decisions

---

# Why Project Memory?

Without project memory, AI only knows what you provide in the current prompt.

With project memory, AI starts each task with a shared understanding of the project.

Benefits include:

* Better consistency
* Less repeated information
* Better code generation
* Better architecture decisions
* Faster prompts

---

# The `.ai` Directory

Create a directory inside every project:

```text
.ai/
```

This directory stores all AI-related project knowledge.

It should be committed to version control unless it contains sensitive information.

---

# Recommended Structure

```text
.ai/

project.md

architecture.md

rules.md

tasks.md

decisions.md

glossary.md

stack.md

features.md

progress.md

known-issues.md
```

You may add more files later as your project grows.

---

# project.md

Purpose:

Describe the project.

Include:

* Project name
* Objective
* Main features
* Target users
* Current version

This is the first file AI should understand.

---

# architecture.md

Describe:

* Folder structure
* Module relationships
* Data flow
* Navigation
* API architecture
* Design principles

Keep diagrams optional.

---

# rules.md

Store coding standards.

Examples:

* Always use TypeScript.
* Functional components only.
* No inline styles.
* Reuse existing utilities.
* Keep services reusable.

This keeps AI responses consistent.

---

# tasks.md

Track active work.

Examples:

* Current feature
* Current bug
* Upcoming tasks
* Blockers

Update this file regularly.

---

# decisions.md

Record important engineering decisions.

Examples:

* Why Expo Router was selected
* Why Zustand replaced Redux
* Why PostgreSQL was chosen

This prevents AI from suggesting previously rejected approaches.

---

# glossary.md

Define project terminology.

Examples:

* Customer
* Organization
* Workspace
* Session
* Subscription

AI can use consistent terminology throughout the project.

---

# stack.md

Describe the technology stack.

Example:

* React Native
* Expo
* TypeScript
* Node.js
* Supabase
* Zustand

Include major versions when helpful.

---

# features.md

Maintain a feature list.

Example:

* Authentication
* Chat
* Notifications
* Payments
* Settings

Briefly describe each feature.

---

# progress.md

Track development progress.

Examples:

* Completed
* In Progress
* Planned
* Blocked

This helps AI understand the current state of the project.

---

# known-issues.md

Document known problems.

Examples:

* Current bugs
* Temporary workarounds
* Technical debt
* Performance issues

AI should avoid suggesting solutions that are already known to be unsuitable.

---

# Updating Project Memory

Update these files whenever:

* New architecture is introduced
* New features are added
* Coding standards change
* Important decisions are made

Treat Project Memory like documentation.

---

# Suggested Workflow

```text
Project Updated

↓

Update .ai Files

↓

Commit Changes

↓

Use AI

↓

Generate Better Responses
```

Keeping Project Memory current improves every future AI interaction.

---

# What Not to Store

Avoid storing:

* Passwords
* API Keys
* Access Tokens
* Personal Information
* Sensitive Customer Data

Project Memory should never contain secrets.

---

# Version Control

Recommended:

Commit `.ai/` to Git.

This allows the entire team to share the same project knowledge.

If necessary, exclude individual files containing temporary notes.

---

# AI Prompt Example

```text
Read the files inside the .ai directory before answering.

Follow the project architecture.

Follow the coding rules.

Reuse existing components.

Keep the implementation consistent with previous decisions.
```

This simple instruction gives AI valuable context before any coding task.

---

# Common Mistakes

Avoid:

* Never updating Project Memory
* Writing overly long documents
* Duplicating information
* Storing secrets
* Ignoring architectural decisions

Keep the files concise and current.

---

# Best Practices

* Keep each file focused on one topic.
* Update documentation alongside code.
* Prefer short bullet points over long paragraphs.
* Remove outdated information.
* Review Project Memory during major releases.

---

# Verification Checklist

Confirm:

* You understand the purpose of Project Memory.
* You created the `.ai` directory.
* You know the purpose of each file.
* You update Project Memory as the project evolves.
* You avoid storing sensitive information.

---

# Developer Notes

Project Memory is not designed for AI alone.

It also improves onboarding, documentation and team communication.

Treat it as a living knowledge base.

The more accurate and current it is, the more useful every AI assistant becomes.

---

# References

* Markdown Documentation
* Software Architecture Documentation
* Documentation-as-Code Practices

---

# Next Chapter

Continue with:

**25 - Context Management**

The next chapter explains how to provide the right amount of context to AI, how to avoid overwhelming smaller local models, and how to keep conversations focused while working on large projects.
