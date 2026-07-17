# 21 - Debugging with AI

# Quick Summary

Debugging is one of the most valuable uses of AI.

The best results come from treating AI as a debugging partner rather than asking it to guess the solution.

Always collect evidence before asking AI for help.

---

# Goal

After completing this chapter you will:

* Debug applications more efficiently
* Ask better debugging questions
* Identify root causes faster
* Interpret stack traces
* Reduce debugging time
* Avoid common debugging mistakes

---

# Debugging Philosophy

Fix the root cause.

Do not hide symptoms.

Temporary fixes often create larger problems later.

---

# Debugging Workflow

Always follow this workflow:

```text
Observe

↓

Reproduce

↓

Collect Evidence

↓

Analyze

↓

Ask AI

↓

Implement Fix

↓

Test

↓

Commit
```

Skipping steps usually increases debugging time.

---

# Step 1 - Observe

Before changing code:

* Read the error
* Understand what failed
* Identify where it failed
* Check recent changes

Never modify code before understanding the problem.

---

# Step 2 - Reproduce

Ensure the problem can be reproduced consistently.

Record:

* Steps
* Device
* Platform
* Environment
* Expected behavior
* Actual behavior

A reproducible bug is much easier to solve.

---

# Step 3 - Collect Evidence

Gather useful information:

* Error messages
* Stack traces
* Console logs
* API responses
* Screenshots
* Device information

The more evidence you provide, the better AI performs.

---

# Step 4 - Analyze

Ask yourself:

* What changed?
* Is it reproducible?
* Is it platform-specific?
* Is it data-related?
* Is it configuration-related?

Only after this should AI be involved.

---

# Step 5 - Ask AI

Provide:

* Technology stack
* Framework version
* Error message
* Relevant code
* Expected behavior
* Actual behavior

Avoid sending unrelated files.

---

# Example Debug Prompt

```text
Role:
Senior React Native Debugging Engineer

Stack:
Expo SDK (Latest Stable)
React Native
TypeScript

Problem:
Application crashes after login.

Expected:
Navigate to Home Screen.

Actual:
Application crashes immediately.

Error:
<Paste complete error>

Relevant Code:
<Paste only the related files>

Requirements:
Find the root cause.
Explain the issue.
Provide the safest fix.
Do not rewrite unrelated code.
```

---

# Reading Stack Traces

Focus on:

* First relevant error
* File name
* Function name
* Line number

Many later errors are only side effects.

---

# Logging

Useful logs include:

* Console output
* API requests
* API responses
* State values
* Navigation events

Avoid logging sensitive data.

---

# React Native Debugging

AI is useful for:

* Navigation errors
* State issues
* AsyncStorage problems
* Expo API issues
* Rendering problems
* Performance issues

Always mention whether the issue occurs on Android, iOS or both.

---

# Backend Debugging

Provide:

* Request
* Response
* Status Code
* Headers
* Logs
* Database errors

Backend debugging requires complete request context.

---

# Python Debugging

Include:

* Exception
* Traceback
* Input
* Expected output
* Actual output

Keep examples minimal but complete.

---

# Performance Debugging

Collect:

* CPU usage
* Memory usage
* Slow screens
* Large lists
* Slow API calls

Optimize only after identifying the bottleneck.

---

# Binary Search Technique

When a large change introduces a bug:

* Disable half the changes.
* Test.
* Narrow the search.
* Repeat.

This often finds the issue faster than random edits.

---

# Compare Working vs Broken

Ask AI to compare:

* Working implementation
* Broken implementation

Differences are often easier to identify than isolated errors.

---

# Verify the Fix

After applying the solution:

* Test again
* Verify edge cases
* Check related features
* Review logs

Never assume the first fix is complete.

---

# Common Mistakes

Avoid:

* Asking AI before reproducing the issue
* Sharing incomplete error messages
* Sending unrelated code
* Applying fixes without understanding them
* Ignoring regression testing

---

# Best Practices

* Reproduce every bug.
* Keep logs meaningful.
* Ask one debugging question at a time.
* Test every fix.
* Commit only after verification.

---

# Verification Checklist

Confirm:

* You follow a structured debugging workflow.
* You collect evidence before asking AI.
* You provide complete context.
* You verify every fix.
* You understand the importance of root cause analysis.

---

# Developer Notes

The quality of debugging depends more on the quality of the information provided than on the AI model itself.

A smaller local model with excellent context often performs better than a larger model with vague prompts.

Think like an investigator before thinking like a programmer.

---

# References

* Official documentation for your framework
* Debugging guides for React, React Native, Node.js and Python
* Browser and platform debugging tools

---

# Next Chapter

Continue with:

**22 - Code Review with AI**

The next chapter explains how to use AI as a code reviewer, identify maintainability issues, improve readability, detect security concerns and provide structured review feedback before merging changes.
