# 26 - Project Rules

# Quick Summary

Project Rules define how AI should behave while working on your project.

Instead of repeating coding standards in every prompt, maintain a single rule file that can be reused across development sessions and AI tools.

Project Rules improve consistency, reduce repetitive instructions and help AI generate code that matches your project's standards.

---

# Goal

After completing this chapter you will:

* Understand Project Rules
* Build reusable AI instructions
* Improve consistency
* Reduce repetitive prompts
* Standardize development practices
* Share coding standards across the team

---

# What Are Project Rules?

Project Rules are permanent instructions that describe how code should be written inside a project.

Unlike prompts, rules remain stable over time.

They represent the project's engineering standards.

---

# Why Use Project Rules?

Benefits include:

* Consistent code generation
* Fewer repeated instructions
* Better maintainability
* Faster prompts
* Easier onboarding
* Shared team standards

---

# Location

Store the rules here:

```text
.ai/rules.md
```

Keep this file under version control.

---

# Recommended Structure

```text
Architecture Rules

Coding Rules

Naming Rules

Folder Rules

Framework Rules

Database Rules

Testing Rules

Git Rules

Documentation Rules

Performance Rules

Security Rules

AI Behavior Rules
```

Organize related rules together.

---

# Architecture Rules

Examples:

* Follow the existing project architecture.
* Do not introduce new architectural patterns without approval.
* Reuse existing services whenever possible.
* Keep business logic outside UI components.
* Keep modules loosely coupled.

---

# Coding Rules

Examples:

* Use TypeScript.
* Avoid the `any` type.
* Prefer readable code over clever code.
* Write small functions.
* Keep files focused on one responsibility.

---

# Naming Rules

Examples:

* Use PascalCase for components.
* Use camelCase for variables.
* Use descriptive names.
* Avoid abbreviations unless they are widely understood.

Consistency improves readability.

---

# Folder Rules

Examples:

* Keep reusable components in the components directory.
* Store business logic in services.
* Place utility functions in utils.
* Do not duplicate folder structures unnecessarily.

---

# Framework Rules

Examples:

* Use functional React components.
* Reuse existing hooks.
* Keep navigation unchanged unless required.
* Follow the existing state management solution.

---

# Database Rules

Examples:

* Validate all input.
* Never expose secrets.
* Keep queries reusable.
* Use migrations for schema changes.
* Avoid duplicate database logic.

---

# Testing Rules

Examples:

* Test new features.
* Test bug fixes.
* Preserve existing behavior.
* Do not remove tests without justification.

---

# Git Rules

Examples:

* Commit small changes.
* Write meaningful commit messages.
* Create feature branches.
* Never commit secrets.
* Review before merging.

---

# Documentation Rules

Examples:

* Update documentation when features change.
* Keep README current.
* Document public APIs.
* Remove outdated information.

---

# Performance Rules

Examples:

* Optimize only after measurement.
* Avoid unnecessary re-renders.
* Reuse expensive calculations.
* Lazy load large resources where appropriate.

---

# Security Rules

Examples:

* Validate all user input.
* Store secrets securely.
* Use least-privilege principles.
* Sanitize external data.
* Never hardcode credentials.

---

# AI Behavior Rules

Examples:

* Explain significant changes.
* Preserve existing functionality.
* Do not rewrite unrelated code.
* Prefer incremental improvements.
* Ask for clarification when requirements are ambiguous.

These rules define how you expect AI to collaborate.

---

# Example Prompt

```text
Read the following before answering:

.ai/project.md
.ai/rules.md
.ai/architecture.md

Follow every applicable project rule.

Do not introduce new dependencies unless necessary.

Keep the existing folder structure.
```

---

# Updating Rules

Review Project Rules when:

* Adopting new technologies
* Changing architecture
* Updating coding standards
* Completing major refactors

Rules should evolve with the project.

---

# Common Mistakes

Avoid:

* Writing vague rules
* Duplicating rules
* Contradictory instructions
* Outdated standards
* Tool-specific rules when avoidable

---

# Best Practices

* Keep rules concise.
* Make rules measurable.
* Review rules regularly.
* Version control the file.
* Prefer stable engineering principles over temporary preferences.

---

# Verification Checklist

Confirm:

* You understand the purpose of Project Rules.
* You know where to store them.
* You can distinguish rules from prompts.
* You know how to update rules.
* You understand why measurable rules are more effective.

---

# Developer Notes

Project Rules are one of the most valuable long-term investments for AI-assisted development.

A clear set of engineering standards helps every developer—and every AI assistant—produce more consistent work.

The goal is not to restrict creativity, but to reduce unnecessary variation.

---

# References

* Clean Code
* Software Engineering Best Practices
* Official framework style guides

---

# Next Chapter

Continue with:

**27 - Automation**

The next chapter explains how to automate repetitive development tasks using AI, scripts and local tooling, including code generation, documentation updates, project setup, validation and daily developer workflows.
