# 13 - Prompt Engineering

# Quick Summary

Prompt engineering is the process of communicating effectively with AI.

A clear prompt produces better code, fewer mistakes and more consistent responses.

Learning to write good prompts is one of the highest-impact skills for AI-assisted development.

---

# Goal

After completing this chapter you will:

* Understand prompt structure
* Write better development prompts
* Get more accurate AI responses
* Reduce hallucinations
* Improve consistency
* Build reusable prompt templates

---

# What Is a Prompt?

A prompt is the instruction you give to an AI model.

The quality of the prompt directly affects the quality of the response.

Think of it as writing a technical specification for another developer.

---

# Good Prompt Principles

A good prompt should be:

* Clear
* Specific
* Focused
* Complete
* Easy to understand

Avoid vague or ambiguous requests.

---

# Prompt Structure

A simple prompt usually contains:

```text
Role

Task

Context

Requirements

Expected Output
```

Following a consistent structure improves response quality.

---

# Example Structure

```text
Role:
Senior React Native Developer

Task:
Create a login screen.

Context:
Expo SDK 54 with TypeScript.

Requirements:
Responsive layout
Form validation
Reusable components

Output:
Production-ready code
```

---

# Give Context

Always provide context.

Instead of:

```text
Fix this.
```

Use:

```text
Fix this React Native component.

Expo SDK 54.

TypeScript.

Do not change the existing API.

Explain the bug before providing the solution.
```

The more relevant context you provide, the better the result.

---

# One Task Per Prompt

Avoid asking AI to solve many unrelated problems.

Bad example:

```text
Create login.

Fix API.

Optimize database.

Write documentation.

Generate tests.
```

Better:

```text
Create the login screen first.
```

Complete one task before moving to the next.

---

# Be Specific

Instead of:

```text
Improve my app.
```

Use:

```text
Improve the performance of this FlatList.

Avoid unnecessary re-renders.

Keep the existing functionality unchanged.
```

Specific requests produce better results.

---

# Mention Technologies

Always specify the technologies being used.

Example:

* React
* React Native
* Expo
* Node.js
* Express
* Python
* TypeScript

Never assume the model knows your stack.

---

# Mention Versions

When relevant, include versions.

Example:

```text
React Native 0.82

Expo SDK 54

Node.js 24

TypeScript 5.x
```

Version information helps avoid outdated solutions.

---

# Define Constraints

Tell the AI what it should not change.

Examples:

* Keep the API unchanged.
* Do not rename variables.
* Preserve TypeScript types.
* Do not add unnecessary libraries.
* Follow existing folder structure.

Constraints reduce unwanted modifications.

---

# Ask for Explanations

Instead of requesting only code, ask for a brief explanation.

Example:

```text
Explain the root cause.

Show the solution.

Explain why the solution works.
```

This improves understanding and debugging.

---

# Break Large Problems Into Steps

Large requests should be divided into smaller tasks.

Example workflow:

```text
Step 1

Create authentication API.

↓

Step 2

Create login screen.

↓

Step 3

Connect API.

↓

Step 4

Handle errors.

↓

Step 5

Write tests.
```

Smaller tasks usually produce better results.

---

# Request Production-Ready Code

When appropriate, specify quality expectations.

Example:

```text
Write production-ready code.

Use TypeScript.

Follow best practices.

Add comments where necessary.

Handle errors properly.
```

---

# Review AI Output

Never assume AI is always correct.

Always:

* Read the code.
* Test the implementation.
* Check edge cases.
* Verify logic.
* Review security implications.

AI is a development assistant, not a replacement for testing.

---

# Reusable Prompt Pattern

Use this template for most coding tasks.

```text
Role:
Senior Software Engineer

Task:
<Describe the task>

Project:
<React / React Native / Node.js / Python>

Requirements:
<List requirements>

Constraints:
<List restrictions>

Output:
<Expected result>
```

---

# Common Prompt Types

Examples include:

* Code Generation
* Bug Fixing
* Code Review
* Refactoring
* Documentation
* Testing
* Optimization
* Architecture
* API Design

We will create reusable templates for each later in this guide.

---

# Common Mistakes

Avoid:

* Very short prompts
* Multiple unrelated requests
* Missing project context
* Missing framework information
* Asking for an entire application in one prompt

---

# Best Practices

* Be specific.
* Use structured prompts.
* Keep prompts focused.
* Reuse successful prompts.
* Build a personal prompt library.
* Review every AI response.

---

# Verification Checklist

Confirm:

* You understand prompt structure.
* You know how to provide context.
* You know how to define constraints.
* You understand why large tasks should be split.
* You can create a structured prompt.

---

# Developer Notes

Think of AI as a senior teammate joining your project.

The more context and constraints you provide, the more useful the responses become.

Good prompts reduce revisions, save time and produce more maintainable code.

---

# References

* Official Prompt Engineering Guides
* Model documentation for your selected AI model
* AI provider best practices

---

# Next Chapter

Continue with:

**14 - AI Coding Workflows**

The next chapter explains practical AI-assisted development workflows for React, React Native, Node.js and Python. You'll learn how to build features, debug issues, review code and refactor projects using local AI in a structured and repeatable way.
