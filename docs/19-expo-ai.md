# 19 - Expo AI Workflow

# Quick Summary

Expo provides one of the fastest ways to build React Native applications.

Combined with AI, Expo enables rapid development while maintaining a clean, consistent and production-ready workflow.

This chapter explains how AI should assist during the complete Expo development lifecycle.

---

# Goal

After completing this chapter you will:

* Build Expo applications efficiently
* Use AI throughout the development lifecycle
* Maintain consistent project structure
* Generate production-ready features
* Reduce repetitive development work

---

# Recommended Stack

This guide recommends:

* Expo SDK (Latest Stable)
* TypeScript
* Expo Router (recommended)
* React Navigation (if required)
* ESLint
* Prettier
* EAS Build

Use the latest stable versions whenever possible.

---

# Development Philosophy

AI should follow your project architecture.

Do not allow AI to introduce multiple navigation systems, duplicate utilities or inconsistent folder structures.

Keep the project predictable.

---

# Typical Workflow

```text
Requirement

↓

Planning

↓

Screen

↓

Components

↓

Hooks

↓

API Integration

↓

Testing

↓

Build

↓

Documentation

↓

Commit
```

---

# Project Structure

Example structure:

```text
app/

components/

hooks/

services/

utils/

types/

constants/

assets/

scripts/

docs/
```

Provide this structure whenever AI generates new files.

---

# Creating New Features

Generate one feature at a time.

Examples:

* Authentication
* Dashboard
* Profile
* Settings
* Notifications
* Chat
* Search

Avoid requesting multiple unrelated features in one prompt.

---

# Navigation

AI can assist with:

* Expo Router
* Dynamic routes
* Protected routes
* Deep linking
* Layouts
* Tabs
* Stacks
* Modals

Always verify navigation manually.

---

# Components

Generate reusable:

* Buttons
* Cards
* Inputs
* Lists
* Modals
* Empty States
* Loading Components
* Error Views

Prefer composition over duplication.

---

# Hooks

Generate focused hooks for:

* Authentication
* API Requests
* Theme
* Network
* Pagination
* Permissions
* Device Information

One responsibility per hook.

---

# API Integration

AI can generate:

* API clients
* Service layer
* Error handling
* Request wrappers
* Retry logic

Keep networking outside UI components.

---

# Expo APIs

Common Expo modules include:

* Camera
* Image Picker
* Notifications
* Secure Store
* File System
* Location
* Clipboard
* Device
* Linking

Always specify which Expo module you are using when prompting AI.

---

# Environment Variables

Store configuration separately.

Examples:

* API URL
* Feature Flags
* Analytics Keys

Never hardcode secrets.

---

# Assets

Organize assets clearly.

Examples:

* Images
* Fonts
* Icons
* Lottie Animations

Avoid duplicate assets.

---

# Builds

AI can assist with:

* Development builds
* Preview builds
* Production builds
* Build configuration
* Build troubleshooting

Always verify build output before releasing.

---

# OTA Updates

Use AI to help:

* Plan update strategy
* Prepare release notes
* Verify compatibility
* Document changes

Test updates before publishing.

---

# Performance

Ask AI to optimize:

* FlatList
* Images
* Re-renders
* Memoization
* Lazy loading
* Bundle size

Optimize only after identifying real bottlenecks.

---

# Error Handling

Improve:

* User feedback
* Retry options
* Loading states
* Offline handling
* Unexpected failures

Handle errors consistently across the application.

---

# Documentation

Generate:

* Setup guides
* Feature documentation
* Build notes
* Deployment notes
* Release notes

Documentation should evolve with the project.

---

# AI Prompt Example

```text
Role:
Senior Expo Developer

Task:
Create a reusable Profile Screen.

Project:
Expo SDK (Latest Stable)
TypeScript
Expo Router

Requirements:
Responsive
Reusable Components
API Integration
Loading State
Error Handling

Constraints:
Do not change navigation structure.
Follow the existing folder organization.

Output:
Production-ready implementation with explanation.
```

---

# Common Mistakes

Avoid:

* Mixing Expo Router with unrelated navigation patterns
* Duplicating components
* Ignoring existing project structure
* Skipping testing on real devices
* Accepting AI output without review

---

# Best Practices

* Build one feature at a time.
* Keep components reusable.
* Keep hooks focused.
* Reuse utilities.
* Test every screen.
* Review every AI suggestion.

---

# Verification Checklist

Confirm:

* You understand the recommended project structure.
* You generate one feature at a time.
* You provide project context.
* You review generated code.
* You test before every commit.

---

# Developer Notes

Expo removes much of the complexity of React Native development.

Use AI to accelerate implementation, not to replace engineering decisions.

A consistent Expo project is easier to maintain and easier for AI to understand.

---

# References

* Official Expo Documentation
* Expo Router Documentation
* EAS Build Documentation
* React Native Documentation

---

# Next Chapter

Continue with:

**20 - Firebase & Supabase AI Workflow**

The next chapter explains how to use AI when building applications with Firebase and Supabase, including authentication, databases, storage, real-time features, security rules and backend integrations.
