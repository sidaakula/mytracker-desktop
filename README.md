# 📘 My Tracker Desktop

[![Latest Release](https://img.shields.io/github/v/release/sidaakula/mytracker-desktop?color=emerald&style=for-the-badge&logo=github)](https://github.com/sidaakula/mytracker-desktop/releases)
[![Total Downloads](https://img.shields.io/github/downloads/sidaakula/mytracker-desktop/total?color=indigo&style=for-the-badge&logo=github)](https://github.com/sidaakula/mytracker-desktop/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-blue.svg?style=for-the-badge)](https://microsoft.com)
[![Local AI](https://img.shields.io/badge/AI-Gemini%20|%20OpenAI%20|%20Ollama-green.svg?style=for-the-badge)](https://ollama.ai)

**My Tracker Desktop** is an intelligent, privacy-first personal task manager that automatically collects school assignments, work tasks, emails, and reminders, converts them into actionable items using **AI**, and presents them as **interactive floating sticky notes** directly on your Windows desktop.

It now features a **Chatbot** and an easy **Setup Wizard**!

---

## 📥 Download & Quick Start Guide

### 1. Installation
Because MyTracker is a portable application, there is no complicated installer! 
- Download **`MyTracker.exe`** from **[Latest Releases](https://github.com/sidaakula/mytracker-desktop/releases)**.
- Open your **Downloads** folder and double-click **`MyTracker.exe`** to run it.
  > [!NOTE]
  > **Windows Defender Warning:** Since this is a brand-new indie app, Windows SmartScreen might pop up saying "Windows protected your PC." 
  > If this happens, click **More info**, and then click **Run anyway**.
  >
  > **Chromebook / Mac Users:** The `.exe` file only works on Windows! If you are using a Chromebook, you must enable Linux (Beta) in your settings, download the source code, open your Linux terminal, and run `./setup_chromebook.sh`.

### 2. The Setup Wizard
Since this is your first time opening the app, a friendly 4-step wizard will appear. It will ask for:
- The Student's Name
- The Student's Gmail and **App Password**.
  > [!IMPORTANT]
  > **How to get an App Password:** Do NOT use your normal Gmail password. Google blocks apps from logging in this way.
  > 1. Go to your Google Account (myaccount.google.com)
  > 2. Click **Security** on the left.
  > 3. Turn on **2-Step Verification** (if it isn't already).
  > 4. Search for **App Passwords** in the top search bar.
  > 5. Type "MyTracker" as the app name and click **Create**.
  > 6. Google will give you a 16-letter code. Copy and paste that code without spaces into the wizard!
- The Parent's Email (for automated grading and completion notifications).
- Your preferred AI (Gemini AI, OpenAI, or Ollama) and your API Key.
  > [!TIP]
  > **How to get a Gemini API Key (Free):** Go to [Google AI Studio](https://aistudio.google.com/app/apikey), sign in, and click **Create API Key**.
  >
  > **How to use Ollama (100% Offline):** Install [Ollama](https://ollama.com/download), run `ollama run llama3` in command prompt, and leave the API key blank in the wizard!

### 3. Using the App
- Once the wizard is complete, it minimizes to the System Tray. 
- Right-click the **🎯 tray icon** to open the **Chatbot**, trigger an instant email sync, or edit settings.
- To create tasks via email, just send an email to the student's inbox starting with `MyTracker:` (e.g. `MyTracker: Create a 20 min Music task every Friday`).
