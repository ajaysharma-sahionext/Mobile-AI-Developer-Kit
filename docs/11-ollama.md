# 11 - Ollama

# Quick Summary

Ollama is the AI engine used throughout this project.

It is responsible for downloading, managing and running local Large Language Models (LLMs) directly on your Android device through the Linux environment provided by Termux.

Everything related to AI in this guide depends on Ollama.

---

# Goal

After completing this chapter you will:

* Understand how Ollama works
* Install Ollama
* Verify the installation
* Download AI models
* Run models locally
* Manage installed models
* Understand memory usage
* Select the correct models for your hardware
* Optimize performance
* Troubleshoot common problems

---

# What is Ollama?

Ollama is a lightweight runtime for Large Language Models.

Instead of sending your code to cloud services, Ollama allows supported AI models to run locally on your device.

This provides better privacy, offline access and full control over your development environment.

---

# Why We Chose Ollama

Reasons:

* Simple command-line interface
* Large model library
* Active community
* Cross-platform
* Easy model management
* Beginner friendly

It is currently one of the easiest ways to work with local AI.

---

# How Ollama Fits Into Our Workflow

```text
VS Code Android
        │
        ▼
     Edit Code
        │
        ▼
     Save Files
        │
        ▼
      Termux
        │
        ▼
      Ollama
        │
        ▼
    Local AI Model
        │
        ▼
AI Response / Code Generation
```

---

# Hardware Expectations

This guide is optimized for:

* Android 15+
* Android 16
* 8GB RAM
* Snapdragon 8 Series

Devices with 12GB or more RAM will provide a noticeably better experience.

---

# Understanding Local AI

Unlike cloud AI services, local models use your phone's:

* CPU
* RAM
* Storage

No internet connection is required after the model has been downloaded.

---

# Storage Requirements

Plan storage carefully.

Approximate requirements:

| Model Size      | Recommended Free Storage |
| --------------- | -----------------------: |
| 2B–4B           |                  8–15 GB |
| 7B–8B           |                 15–25 GB |
| Multiple Models |                 30–50 GB |

Leave additional free space for projects and updates.

---

# RAM Planning

General expectations:

| RAM   | Recommendation                        |
| ----- | ------------------------------------- |
| 6GB   | Small models only                     |
| 8GB   | 3B–4B models (recommended target)     |
| 12GB  | 7B models become practical            |
| 16GB+ | Larger models and better multitasking |

Do not choose models based only on popularity.

Choose models that fit your hardware.

---

# Installing Ollama

Install Ollama using the latest method supported for Android and Termux.

Because installation methods may change over time, always follow the current official instructions when performing the installation.

After installation, verify that the executable is available.

Example:

```bash
ollama --version
```

If a version number is displayed, the installation was successful.

---

# Verify the Service

Confirm that Ollama can start correctly.

Example:

```bash
ollama list
```

If no models are installed yet, an empty list is expected.

---

# Understanding Models

Ollama itself is **not** an AI model.

Think of Ollama as the engine.

Models are downloaded separately and can be added or removed whenever needed.

---

# Download Your First Model

Example:

```bash
ollama pull gemma3:4b
```

Or another model recommended later in this guide.

Wait for the download to complete before continuing.

---

# List Installed Models

```bash
ollama list
```

This displays every model currently available on your device.

---

# Run a Model

Example:

```bash
ollama run gemma3:4b
```

You can immediately begin asking questions after the model loads.

---

# Exit a Session

To leave an interactive session:

```text
Ctrl + D
```

or

```text
/bye
```

depending on the model/runtime behavior.

---

# Remove a Model

If storage becomes limited:

```bash
ollama rm MODEL_NAME
```

Only remove models you no longer need.

---

# Update a Model

Pull the model again.

```bash
ollama pull MODEL_NAME
```

Ollama downloads the latest available version if one exists.

---

# Model Quantization

Many models are available in different quantizations.

Examples:

* Q2
* Q3
* Q4
* Q5
* Q6
* Q8

General guidance:

* Lower quantization → Smaller, faster, lower quality.
* Higher quantization → Better quality, more RAM and storage.

For 8GB phones, **Q4** is usually the best balance.

---

# Choosing Models for 8GB RAM

Recommended priorities:

### Primary Coding

* Qwen Coder (small quantized variant)

### General Assistant

* Gemma (4B class)

### Fast Utility

* 2B–3B lightweight model

Avoid downloading many large models at the beginning.

---

# Context Window

The context window determines how much information the model can remember during a conversation.

Longer context requires more memory.

For daily mobile development, shorter focused conversations usually produce better results.

---

# Prompting Tips

Good prompts should:

* Be specific.
* Include the programming language.
* Mention the framework.
* Describe the expected output.
* Request only one task at a time.

Large requests should be divided into smaller steps.

---

# Performance Tips

For the best experience:

* Close unnecessary applications.
* Keep the device cool.
* Use one AI model at a time.
* Keep at least 20GB free storage.
* Charge the phone during long AI sessions.

---

# Battery Considerations

Local AI consumes more power than normal applications.

Expect:

* Higher battery usage
* Increased CPU load
* Additional heat during long sessions

This behavior is normal.

---

# Model Management Strategy

Instead of installing many models:

Keep:

* One coding model
* One general assistant
* One lightweight utility model

This provides the best balance between capability and storage usage.

---

# Best Practices

* Update Ollama periodically.
* Remove unused models.
* Keep conversations focused.
* Organize projects before asking AI.
* Prefer smaller models that run smoothly.

---

# Common Mistakes

Avoid:

* Installing models larger than your hardware can handle.
* Running multiple models simultaneously.
* Filling device storage completely.
* Expecting desktop-class performance.
* Asking the model to generate an entire application in one prompt.

---

# Troubleshooting

## Model Runs Slowly

Possible causes:

* Insufficient RAM
* Large model
* Background applications
* Thermal throttling

Use a smaller model if necessary.

---

## Download Interrupted

Retry the download.

Ollama generally resumes safely.

---

## Out of Storage

Remove unused models or free additional storage before downloading another model.

---

## Model Not Found

Verify the model name.

List installed models:

```bash
ollama list
```

---

# Verification Checklist

Confirm:

* ✅ Ollama installed
* ✅ Version verified
* ✅ First model downloaded
* ✅ Model starts successfully
* ✅ Interactive chat works
* ✅ Model list available
* ✅ Model removal understood

If every item is complete, your local AI engine is ready.

---

# Developer Notes

Do not chase the largest available model.

For mobile development, responsiveness is usually more valuable than raw benchmark performance.

A smaller model that answers in a few seconds is often more productive than a larger model that takes significantly longer to respond.

Throughout the rest of this guide, every AI workflow will be optimized around this principle.

---

# References

* Official Ollama Documentation
* Official Ollama Model Library
* Official GGUF Format Documentation (for background knowledge)

---

# Next Chapter

Continue with:

**12 - AI Models & Recommendations**

The next chapter compares the best AI models available for Android in 2026, explains which models are best for React, React Native, Node.js and Python development, and provides hardware-based recommendations for 8GB, 12GB and 16GB devices.
