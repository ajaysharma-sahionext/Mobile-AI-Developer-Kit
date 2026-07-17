# 25 - Context Management

# Quick Summary

AI performs best when it receives the right amount of context.

Too little context leads to incorrect assumptions.

Too much context wastes the model's context window and often reduces response quality.

This chapter explains how to provide efficient, structured context for local AI models.

---

# Goal

After completing this chapter you will:

* Understand AI context
* Reduce unnecessary prompts
* Improve response quality
* Optimize local model performance
* Keep conversations focused
* Build reusable context patterns

---

# What is Context?

Context is all the information the AI uses before generating a response.

Examples include:

* Current prompt
* Previous conversation
* Project Memory
* Code snippets
* Error messages
* Requirements

The quality of the context directly affects the quality of the response.

---

# Why Context Matters

Good context helps AI:

* Understand the task
* Follow project standards
* Avoid incorrect assumptions
* Produce consistent code
* Reduce unnecessary explanations

---

# The Context Pyramid

Provide information in this order:

```text
Current Task

↓

Relevant Code

↓

Related Files

↓

Project Rules

↓

Architecture

↓

Project Overview
```

Start small.

Only add more information if the model needs it.

---

# Context Levels

## Level 1 — Task

Describe exactly what needs to be done.

Example:

* Fix login bug
* Add search
* Create settings screen

---

## Level 2 — Code

Provide only the code related to the task.

Avoid sending entire projects.

---

## Level 3 — Files

Mention:

* Current file
* Related components
* Services
* APIs

Only include files that influence the task.

---

## Level 4 — Rules

Provide important project rules.

Examples:

* TypeScript only
* Functional components
* Existing folder structure
* Existing API design

---

## Level 5 — Architecture

Describe only the relevant architecture.

Examples:

* Navigation flow
* API layer
* State management
* Database structure

---

## Level 6 — Project

Finally provide:

* Project goal
* Technology stack
* Main features

This information rarely changes.

---

# Small Context Strategy

Instead of:

```text
Analyze my entire project.
```

Use:

```text
Read:

- LoginScreen.tsx
- authService.ts
- authStore.ts

Task:

Fix login validation.

Rules:

Use TypeScript.
Do not change navigation.
Keep API unchanged.
```

Smaller prompts produce more accurate responses.

---

# Context Window

Every model has a limited context window.

As more information is added:

* Memory usage increases
* Response time may increase
* Important information can be pushed out

Prioritize the most relevant information.

---

# Working with Large Projects

Split work into modules.

Example:

```text
Authentication

↓

Dashboard

↓

Settings

↓

Payments

↓

Notifications
```

Avoid asking AI to understand the whole project at once.

---

# Using Project Memory

Reference the `.ai` directory when appropriate.

Examples:

* `.ai/project.md`
* `.ai/rules.md`
* `.ai/architecture.md`

Only include the files relevant to the current task.

---

# Managing Long Conversations

When a conversation becomes lengthy:

* Summarize progress
* Start a new session
* Reuse Project Memory
* Continue with a focused prompt

This often improves response quality.

---

# Context Refresh

When changing features:

* Update Project Memory
* Summarize previous work
* Start the next task with fresh context

Do not rely on the model remembering everything.

---

# AI Prompt Example

```text
Read:

.ai/project.md
.ai/rules.md

Relevant Files:

LoginScreen.tsx
authService.ts

Task:

Implement biometric login.

Constraints:

Do not change authentication APIs.
Reuse existing services.
Use TypeScript.
```

---

# Common Mistakes

Avoid:

* Sending the entire repository
* Including unrelated files
* Mixing multiple features
* Ignoring project rules
* Assuming AI remembers previous sessions

---

# Best Practices

* Keep prompts focused.
* Share only relevant files.
* Reuse Project Memory.
* Break large features into smaller tasks.
* Start new sessions for unrelated work.

---

# Verification Checklist

Confirm:

* You understand context management.
* You know how to prioritize information.
* You avoid unnecessary context.
* You reuse Project Memory effectively.
* You understand the limitations of local models.

---

# Developer Notes

A smaller local model with excellent context often outperforms a much larger model that receives poor or excessive context.

Think like a technical lead preparing a task for another developer.

Provide only the information required to complete that task successfully.

---

# References

* Official documentation for your selected AI model
* Prompt engineering best practices
* Software documentation guidelines

---

# Next Chapter

Continue with:

**26 - Project Rules**

The next chapter explains how to define project-wide coding standards and AI instructions that remain consistent across local models, cloud AI services and future AI development tools.
