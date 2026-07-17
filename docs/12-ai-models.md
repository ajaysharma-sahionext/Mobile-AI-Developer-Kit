# 12 - AI Models & Recommendations

# Quick Summary

Choosing the correct AI model is more important than choosing the largest AI model.

This chapter explains which models are best for different development tasks and how to select the right model for your Android device.

---

# Goal

After completing this chapter you will:

* Understand different AI model categories
* Select models based on available RAM
* Choose the best coding model
* Choose the best reasoning model
* Build an efficient multi-model setup
* Avoid common model selection mistakes

---

# Model Categories

AI models are generally optimized for different tasks.

The most common categories are:

* Coding
* General Assistant
* Reasoning
* Vision
* Mathematics
* Multilingual
* Lightweight

No single model is perfect for every task.

---

# Coding Models

Coding models are optimized for:

* Code generation
* Bug fixing
* Refactoring
* Code explanation
* Documentation
* API development

These should be your primary development models.

---

# General Assistant Models

General assistant models are better for:

* Documentation
* Brainstorming
* Planning
* Architecture
* Learning
* General questions

---

# Reasoning Models

Reasoning models perform better when solving:

* Complex logic
* Multi-step problems
* Algorithm design
* System architecture
* Planning

They may respond more slowly than lightweight models.

---

# Vision Models

Vision models understand images.

Examples:

* UI screenshots
* Diagrams
* Flowcharts
* Design mockups

Vision support depends on both the model and runtime.

---

# Lightweight Models

Lightweight models are useful for:

* Fast responses
* Low RAM devices
* Quick terminal help
* Small coding tasks

These are excellent companions for mobile development.

---

# Recommended Models (2026)

The following families are widely recognized for development tasks:

| Model Family   | Primary Strength     |
| -------------- | -------------------- |
| Qwen Coder     | Software development |
| Gemma          | General assistant    |
| DeepSeek Coder | Programming          |
| Llama          | General purpose      |
| Phi            | Lightweight tasks    |

Model availability and supported variants change over time, so always check the latest Ollama library before downloading.

---

# Hardware Recommendations

## 6GB RAM

Recommended:

* 2B
* 3B

Avoid larger models.

---

## 8GB RAM

Recommended:

* 3B
* 4B

Primary target of this guide.

Provides the best balance between speed and quality.

---

## 12GB RAM

Recommended:

* 7B
* 8B

Excellent balance between capability and responsiveness.

---

## 16GB RAM

Suitable for:

* Larger coding models
* Longer context
* Better multitasking

---

# Recommended Setup (8GB)

Coding Model

* Small Qwen Coder variant

General Assistant

* Gemma 4B class

Utility Model

* Lightweight 2B–3B model

This combination covers most development tasks while remaining responsive.

---

# Recommended Setup (12GB)

Coding

* 7B coding model

General

* Gemma

Utility

* Lightweight assistant

Provides a noticeably better experience for larger projects.

---

# Recommended Setup (16GB+)

Coding

* Larger coding models

Reasoning

* Dedicated reasoning model

Utility

* Small assistant

Suitable for advanced AI workflows.

---

# Development Task Recommendations

| Task          | Recommended Model Type |
| ------------- | ---------------------- |
| React         | Coding                 |
| React Native  | Coding                 |
| Node.js       | Coding                 |
| TypeScript    | Coding                 |
| Python        | Coding                 |
| Debugging     | Coding                 |
| Documentation | General Assistant      |
| Architecture  | Reasoning              |
| Learning      | General Assistant      |

---

# Model Selection Strategy

Do not install every available model.

Instead choose:

* One coding model
* One assistant model
* One lightweight utility model

This keeps storage usage reasonable and simplifies your workflow.

---

# Model Rotation

As new models become available:

* Test them
* Compare them
* Replace older models if they provide clear improvements

Avoid collecting models that you no longer use.

---

# Coding Workflow

Recommended workflow:

```text
Requirement

↓

Coding Model

↓

Generate Code

↓

Review Output

↓

Test

↓

Refactor

↓

Commit
```

---

# Common Mistakes

Avoid:

* Downloading models larger than your device can comfortably run
* Using one model for every task
* Keeping too many unused models
* Ignoring storage limitations
* Judging models only by parameter count

---

# Best Practices

* Keep one primary coding model.
* Keep one assistant model.
* Update models periodically.
* Remove unused models.
* Use focused prompts.
* Test model quality with your own projects.

---

# Verification Checklist

Confirm:

* You understand different model categories.
* You selected models appropriate for your hardware.
* You know which model will be your primary coding assistant.
* You have a plan for managing storage.

---

# Developer Notes

The "best" AI model is the one that helps you finish work efficiently on your hardware.

For an 8GB Android phone, a fast 4B coding model usually provides a better overall experience than a much larger model that struggles with memory or takes significantly longer to respond.

Optimize for productivity, not benchmark rankings.

---

# References

* Official Ollama Model Library
* Official documentation for the selected model families
* Community benchmarks and release notes

---

# Next Chapter

Continue with:

**13 - Prompt Engineering**

The next chapter explains how to write prompts that produce high-quality code, better debugging results, clearer documentation and more reliable AI responses. It will also introduce reusable prompt templates that will later become part of this toolkit.
