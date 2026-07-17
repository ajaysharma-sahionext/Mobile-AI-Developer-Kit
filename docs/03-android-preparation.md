# 03 - Android Preparation

# Quick Summary

Before installing development tools, Android should be optimized for long coding sessions.

This chapter prepares the device by configuring system settings, battery behavior, permissions and storage.

---

# Goal

After completing this chapter your Android device will be ready for:

* Long development sessions
* Running local AI models
* Using Termux
* Running VS Code
* Managing Git repositories

---

# Prerequisites

Make sure you have:

* Android 15 or newer
* Stable internet connection
* At least 25GB free storage
* Battery above 50%

---

# Step 1 — Update Android

Open:

**Settings → System Update**

Install all available updates.

Restart the phone after updating.

---

# Step 2 — Update Google Play System

Open:

**Settings → Security & Privacy → Google Play System Update**

Install updates if available.

Restart the device.

---

# Step 3 — Clean Storage

Remove:

* Unused applications
* Old downloads
* Duplicate files
* Large videos
* Temporary files

Maintain at least **25GB** of free storage.

---

# Step 4 — Organize Storage

Create a clean workspace for future projects.

Recommended folders:

```text
Developer/
Projects/
Downloads/
Documents/
```

Additional folders will be created later.

---

# Step 5 — Battery Optimization

Battery optimization can stop development tools.

For the following applications:

* Termux
* VS Code
* Git clients (if installed)

Set battery mode to:

**Unrestricted** or **Don't Optimize**

The exact option depends on your Android version.

---

# Step 6 — Background Restrictions

Disable aggressive background restrictions for development applications.

This prevents Android from closing active development sessions.

---

# Step 7 — Auto Start

If your phone supports Auto Start management:

Enable Auto Start for:

* Termux
* VS Code

This improves reliability.

---

# Step 8 — Storage Permissions

Development applications should have storage access.

Grant storage permission when requested.

Do not grant unnecessary permissions such as Contacts or Location unless required.

---

# Step 9 — Notification Permissions

Allow notifications for:

* Termux
* VS Code

This helps when running long tasks.

---

# Step 10 — Enable Developer Options

Open:

**Settings → About Phone**

Tap **Build Number** multiple times until Developer Options become available.

The exact location may vary by manufacturer.

---

# Step 11 — Developer Options

Recommended settings:

* USB Debugging → ON
* Stay Awake While Charging → ON
* Logger Buffer Size → Default

Leave all other options unchanged unless you understand their purpose.

---

# Step 12 — Animation Speed

For a smoother experience:

Set:

* Window Animation Scale → 0.5x
* Transition Animation Scale → 0.5x
* Animator Duration Scale → 0.5x

This improves perceived responsiveness.

---

# Step 13 — Display Settings

Recommended:

* Auto Brightness → ON
* Dark Mode → Optional
* Screen Timeout → 10–30 minutes during development

Adjust according to your preference.

---

# Step 14 — Network

Use a stable Wi-Fi connection for:

* Package installation
* AI model downloads
* Git cloning

Mobile data can be used when necessary.

---

# Step 15 — Charging

Large AI models consume significant power.

Recommended:

* Keep battery above 30%.
* Use the original fast charger during long sessions.

Avoid heavy development on very low battery.

---

# Step 16 — Restart

Restart the phone after completing all changes.

This ensures all settings are applied correctly.

---

# Verification

Confirm the following:

* Android is updated
* Google Play System is updated
* 25GB+ free storage available
* Battery optimization disabled for development apps
* Developer Options enabled
* USB Debugging enabled
* Animation scale set to 0.5x
* Phone restarted successfully

If all items are complete, continue to the next chapter.

---

# Troubleshooting

## Phone closes Termux automatically

Disable battery optimization and background restrictions.

---

## Low Storage Warning

Remove unused applications and large files until at least 25GB is available.

---

## Developer Options not visible

Continue tapping the Build Number until Android confirms Developer Mode is enabled.

---

## Animation Settings Missing

Some manufacturers rename or relocate Developer Options.

Use the Settings search feature.

---

# Optional Improvements

These enhancements can be added later:

* Bluetooth keyboard
* Bluetooth mouse
* USB-C hub
* External SSD
* Phone cooling fan

They are helpful but not required.

---

# Notes

Do not root your phone.

This guide is designed to work on standard Android devices without modifying the operating system.

---

# Next Chapter

Continue with:

**04 - Storage Planning**

The next chapter will build a clean directory structure for projects, AI models, scripts, templates, prompts and documentation. A well-organized storage layout makes future automation much easier.
