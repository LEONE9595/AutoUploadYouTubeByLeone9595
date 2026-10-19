# 🚀 AutoUpload YouTube

> **Your YouTube channel, updated automatically.**  
> *Automatic. Free. Self-contained.*  
> **Author:** LEONE9595 | **Current Version:** v1.0.5 Beta

---

## 📌 Project Overview

**AutoUpload YouTube** is a lightweight Windows application designed to fully automate the video upload and scheduling workflow for YouTube creators. It eliminates the tedious manual process of filling out metadata, tags, and scheduling forms on YouTube Studio for series-based content (gameplays, tutorials, vlogs, daily highlights).

Simply place your video files in a designated folder and launch the program: **AutoUpload YouTube** automatically handles batch uploading, custom publication scheduling across days, dynamic title/description formatting, progressive numbering counters, and Google API daily quota limits.

### 🌟 Key Features
* 🤖 **Automated Upload & Scheduling:** Uploads queued videos sequentially and schedules them at customizable daily intervals.
* 🧠 **Smart Metadata Generation:** Automatically parses video filenames (e.g., mode, kill-scores, episode numbers) using regex to build custom titles and descriptions.
* 🔢 **Category Counter Tracking:** Maintains independent progressive counters for each content category, auto-incrementing upon successful uploads.
* ⏳ **Automatic Quota Protection:** Detects Google API daily limit exhaustion, automatically pausing operation and resuming seamlessly upon daily reset.
* 🔔 **System Tray & Desktop Alerts:** Operates in the background with continuous status updates in the system tray and native Windows notifications.
* ⚙️ **Self-Contained Autonomous Installer (`setup_runtime.bat`):** Automatically downloads and installs embedded Python dependencies, creates Desktop shortcuts, and sets up the environment with zero technical background required.
* 🔒 **Local & Secure:** Runs entirely on your local machine with zero third-party cloud servers, interacting directly with official Google API endpoints.

---

## 🆕 Major Updates & Changelog (v1.0.2 to v1.0.5 Beta)

From version 1.0.2 to v1.0.5 Beta, the application evolved from a basic script into a robust, resilient tool featuring an autonomous single-file installer and integrated documentation.

### 🛠️ v1.0.2 Beta — Stability & Feature Enhancements
* **Duplicate Counter Key Fix:** Standardized counter mapping (`Tdm` / `TDM`) in `config/contatori.json` with auto-migration on first boot.
* **Regex Filename Parsing:** Advanced extraction of game modes and statistics with explicit warnings for malformed names.
* **Persistent File Logging:** Introduced `autoupload.log` tracking startups, authentication, uploads, errors, and quota pauses with timestamps.
* **Network Fault Tolerance:** Automatic retry mechanism (up to 3 attempts with progressive delays) for transient HTTP errors (500, 502, 503, 504).
* **Resilient Batch Queue:** Non-fatal video processing errors no longer halt the entire queue.
* **Configurable Tag Management:** Externalized tags and categories into `config/tags_categoria.json`.
* **Batch Time Estimation:** Real-time feedback displaying remaining video counts and ETA estimates for entire batch uploads.
* **Dry-Run Mode (`--dry-run`):** Simulated execution mode to preview titles, descriptions, and scheduling without triggering real API calls.

### ⚡ v1.0.3 Beta — Runtime Automation
* **Autonomous Python Deployment:** `setup_runtime.bat` automatically fetches and configures the embedded Python package on initial launch.
* **Offline Detection:** Skips web downloads if a ready Python runtime environment is already detected locally.

### 🛡️ v1.0.4 Beta — Critical Fixes & Standalone Installer
* **Anti-Double-Upload Protection:** Enhanced file archival resilience post-upload (up to 8 retry attempts) with automatic safe fallback renaming (`.GIA_CARICATO`) to prevent accidental re-uploads.
* **Single-File Autonomous Installer:** `setup_runtime.bat` can completely recreate the entire application directory structure from scratch inside an empty folder.
* **Batch Scripting Improvements:** Resolved output redirection bugs, fixed jump blocks (`GOTO`), and enforced **UTF-8** streams at startup to prevent emoji encoding crashes.
* **Embedded Setup Documentation:** Automatically generates step-by-step Google Cloud API setup guides (`COME_OTTENERE_CREDENZIALI_GOOGLE.txt`).

### 📦 v1.0.5 Beta — Final Consolidation & Distribution
* **End-to-End Verification:** Full test suite verification across fresh environments.
* **PDF Documentation Integration:** Bundled graphical guides detailing operational workflow and credential setup.
* **Minimal Shareable Package (~90 KB):** Streamlined standalone installer package pre-configured with clean initial counters for immediate deployment.

---

## ⚡ Quick Start Guide

1. **Installation:** Download the project folder and double-click `setup_runtime.bat`.
2. **Google Credentials:** Follow the generated instructions inside the `system` folder to place your `client_secret.json`.
3. **Queue Videos:** Move your video files into the `video` folder (e.g., `Conquest_45-12.mp4`).
4. **Run Uploads:** Launch `AVVIA_UPLOAD.bat`, pick your language and start date—the application will manage the rest!

---
*Developed by LEONE9595 | [Website](http://leone9595.altervista.org) | [YouTube Channel](https://youtube.com/user/LEONE9595)*