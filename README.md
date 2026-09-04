# 📘 My Tracker Desktop

[![Latest Release](https://img.shields.io/github/v/release/sidaakula/mytracker-desktop?color=emerald&style=for-the-badge&logo=github)](https://github.com/sidaakula/mytracker-desktop/releases)
[![Total Downloads](https://img.shields.io/github/downloads/sidaakula/mytracker-desktop/total?color=indigo&style=for-the-badge&logo=github)](https://github.com/sidaakula/mytracker-desktop/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-blue.svg?style=for-the-badge)](https://microsoft.com)
[![Local AI](https://img.shields.io/badge/AI-Local%20Ollama%20(100%25%20Private)-green.svg?style=for-the-badge)](https://ollama.ai)

**My Tracker Desktop** is an intelligent, 100% privacy-first personal task manager that automatically collects school assignments, work tasks, emails, and reminders, converts them into actionable items using **Local Ollama AI**, and presents them as **interactive floating sticky notes** directly on your Windows desktop.

---

## 📥 Download & Quick Start Guide

### 1. Download Standalone Windows App
- Download **`MyTracker.exe`** from **[Latest Releases](https://github.com/sidaakula/mytracker-desktop/releases)**.

### 2. Install Local Ollama AI (100% Private Task Extraction)
- Download free from **[ollama.com](https://ollama.com)**.
- Open command prompt and run:
  ```bash
  ollama pull llama3
  ```

### 3. Launch App
- Double-click **`MyTracker.exe`** on Windows 10/11. No Python installation required!
- Right-click tray icon to open **Settings** or trigger instant email sync.

---

## 🔐 Setting Up from GitHub (For New Users)

Because this is a 100% privacy-first application, the creator cannot share their personal Google API keys. If you downloaded the `.exe` from GitHub, you must "Bring Your Own Secrets" (BYOS).

### How to get your own `client_secrets.json`:
1. Go to the **[Google Cloud Console](https://console.cloud.google.com/)** and log in.
2. Create a **New Project** (e.g., "My Tracker").
3. Search for and **Enable** the **Gmail API** and **Google Tasks API** in your project.
4. Go to **APIs & Services > OAuth consent screen**. Choose **External**, fill in the required app name, and add your own email address under the **Test users** section.
5. Go to **Credentials > + CREATE CREDENTIALS > OAuth client ID**.
6. For Application Type, choose **Desktop app** and click Create.
7. Click the **Download JSON** button to download your `client_secrets.json` file.
8. Open the **My Tracker** `.exe`, go to Settings, and select your downloaded JSON file to authenticate.
