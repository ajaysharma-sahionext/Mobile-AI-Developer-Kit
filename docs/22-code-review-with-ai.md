# 22 - Code Review with AI

# Quick Summary

AI can dramatically improve code reviews by identifying bugs, inconsistencies and opportunities for improvement.

However, AI should assist human reviewers rather than replace them.

Use AI to perform structured reviews before every merge or release.

---

# Goal

After completing this chapter you will:

* Review code systematically
* Detect common issues
* Improve maintainability
* Improve readability
* Identify performance concerns
* Catch security problems early

---

# Code Review Philosophy

A good review is not about finding mistakes.

Its purpose is to improve the overall quality of the project.

Every review should make the codebase easier to understand and maintain.

---

# AI Review Workflow

```text
Read Changes

↓

Understand Feature

↓

Review with AI

↓

Validate Suggestions

↓

Apply Improvements

↓

Run Tests

↓

Commit
```

Never apply AI suggestions without verification.

---

# Before Asking AI

Collect the following:

* Feature description
* Relevant files
* Expected behavior
* Existing architecture
* Coding standards

Avoid sending unrelated files.

---

# What AI Should Review

AI should review:

* Logic
* Naming
* Readability
* Reusability
* Error handling
* Performance
* Security
* Type safety
* Documentation

---

# Correctness

Ask AI to verify:

* Business logic
* Edge cases
* Null handling
* State management
* Async operations

Correctness should always be reviewed first.

---

# Security

Review for:

* Secrets
* Authentication
* Authorization
* Input validation
* SQL Injection
* XSS
* Unsafe file handling

Never expose production credentials.

---

# Performance

Review:

* Expensive renders
* Database queries
* Network requests
* Loops
* Memory usage
* Duplicate work

Optimize only when necessary.

---

# Architecture

Verify:

* Folder structure
* Module responsibilities
* Layer separation
* Dependency direction
* Reusability

Avoid introducing inconsistent patterns.

---

# Maintainability

Review:

* Duplicate code
* Large functions
* Complex logic
* Tight coupling
* Magic values

Small improvements reduce future maintenance costs.

---

# Readability

Check:

* Naming
* Formatting
* Comments
* Function length
* File organization

Code should be easy to understand without lengthy explanations.

---

# Documentation

Confirm:

* README updates
* API documentation
* Comments where necessary
* Public function descriptions

Documentation should stay synchronized with implementation.

---

# Testing

Verify:

* Existing tests still pass
* New logic is tested
* Edge cases covered
* Regression risks considered

Testing completes the review process.

---

# React Native Review

Review:

* Component structure
* Hooks
* Navigation
* Re-renders
* FlatList usage
* AsyncStorage
* Expo APIs

---

# Backend Review

Review:

* Routes
* Controllers
* Services
* Validation
* Authentication
* Logging
* Error handling

---

# Python Review

Review:

* Module structure
* Function design
* Error handling
* Dependency usage
* Type hints (if applicable)

---

# AI Review Prompt

```text
Role:
Senior Software Engineer

Task:
Review the following code.

Project:
<Framework>

Review For:
Correctness
Security
Performance
Architecture
Maintainability
Readability

Requirements:
Explain every issue.
Suggest improvements.
Do not rewrite unrelated code.
Prioritize issues by severity.
```

---

# Severity Levels

Classify findings as:

* Critical
* High
* Medium
* Low
* Suggestion

Fix higher-priority issues first.

---

# Common Mistakes

Avoid:

* Reviewing entire repositories at once
* Ignoring project architecture
* Applying every AI suggestion blindly
* Focusing only on style
* Skipping manual testing

---

# Best Practices

* Review small pull requests.
* Keep reviews focused.
* Validate every recommendation.
* Follow project standards.
* Test after applying changes.

---

# Verification Checklist

Confirm:

* You follow a structured review process.
* You classify issues by priority.
* You validate AI suggestions.
* You test after changes.
* You keep architecture consistent.

---

# Developer Notes

The best code reviews improve the project, not the ego of the developer.

AI should help explain *why* something can be improved instead of only suggesting different code.

A structured review process produces better long-term software quality than reviewing only when bugs appear.

---

# References

* Clean Code
* Refactoring
* OWASP Secure Coding Practices
* Official framework style guides

---

# Next Chapter

Continue with:

**23 - Refactoring with AI**

The next chapter explains how to safely refactor applications with AI, reduce technical debt, improve architecture, remove duplication and modernize code while preserving existing behavior.
