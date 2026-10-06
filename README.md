# 🎯 MyTracker User Manual

Welcome to **MyTracker**, the fully automated desktop assistant designed to pull school assignments, chores, and homework from your emails and school portals so you never miss a deadline again. 

This manual will walk you through everything from the first launch to utilizing the interactive AI Chatbot.

> [!TIP]
> You only need to set this up once! After your initial configuration, MyTracker runs silently in the background and does all the heavy lifting automatically.

---

## 1. 🚀 Installation & First Launch

Because MyTracker is a portable application, there is no complicated installer! 

1. Go to the **GitHub Releases** page and download the latest **`MyTracker.exe`** file.
2. Open your **Downloads** folder (or wherever you saved the file) and double-click **`MyTracker.exe`** to run it.
   > [!NOTE]
   > **Windows Defender Warning:** Since this is a brand-new indie app, Windows SmartScreen might pop up saying "Windows protected your PC." 
   > If this happens, click **More info**, and then click **Run anyway**.
   >
   > **Chromebook / Mac Users:** The `.exe` file only works on Windows! If you are using a Chromebook, you must enable Linux first:
   > 1. Go to your Chromebook **Settings**.
   > 2. Click **Advanced** > **Developers**.
   > 3. Next to **Linux development environment**, click **Turn on** and follow the prompts.
   > 4. Once installed, open the **Terminal** app from your app launcher.
   > 5. Paste this exact command and hit Enter:
   > ```bash
   > curl -sSL https://raw.githubusercontent.com/sidaakula/mytracker/main/desktop_agent/setup_chromebook.sh | bash
   > ```
   > It will automatically install everything and create a "MyTracker" icon in your App Launcher!
3. **The Setup Wizard:** Since this is your first time opening the app, a friendly 4-step wizard will appear. It will ask for:
   - The Student's Name
   - A Dedicated Gmail and **App Password**.
     > [!TIP]
     > **RECOMMENDED SETUP:** We highly recommend creating a brand new Gmail account specifically for this app (e.g., `mytrackersid@gmail.com`). Then, log into your child's real school email and set it to **auto-forward** all incoming emails to this new `mytrackersid@gmail.com` address. This keeps everything perfectly organized!
     
     > [!IMPORTANT]
     > **How to get an App Password:** Do NOT use your normal Gmail password. Google blocks apps from logging in this way.
     > 1. Go to your Google Account (myaccount.google.com)
     > 2. Click **Security** on the left.
     > 3. Turn on **2-Step Verification** (if it isn't already).
     > 4. Search for **App Passwords** in the top search bar.
     > 5. Type "MyTracker" as the app name and click **Create**.
     > 6. Google will give you a 16-letter code (e.g., `abcd efgh ijkl mnop`). Copy and paste that code without spaces into the wizard!
   - The Parent's Email (for notifications)
   - Your preferred AI (Gemini AI, OpenAI, or Ollama) and your API Key.
     > [!TIP]
     > **How to get a Gemini API Key (Free):**
     > 1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey).
     > 2. Sign in with any Google account and click **Create API Key**.
     > 3. Copy the key and paste it into the wizard!
     >
     > **How to use Ollama (100% Offline & Private):**
     > 1. Download and install [Ollama](https://ollama.com/download) for Windows.
     > 2. Open Command Prompt and type `ollama run llama3` to download the AI model.
     > 3. Select Ollama in the wizard and leave the API key blank!
   - Links to your School Portals (optional).
4. Once you complete the wizard, it will disappear. MyTracker is now completely invisible so it doesn't distract you!
5. Look down at your **Windows System Tray** (the bottom-right corner of your screen, right next to your clock and WiFi icon). You might need to click the `^` arrow to show hidden icons.
6. You will see a small target icon: **🎯**. This means MyTracker is active and running in the background.

---

## 2. 🤖 The Interactive AI Chatbot

A brand new feature allows the student to directly chat with the app to get help or review their progress.

To open the Chatbot: **Right-Click** the 🎯 target icon in the system tray and click **"Chatbot"**.

- **What it knows:** The chatbot instantly reads your synced homework list, your current class averages, and the app's internal status.
- **What to ask:** 
  - *"What is my ELA grade right now?"*
  - *"What homework do I have due tomorrow?"*
  - *"Show me all completed work from today."*
- **Safety Guardrails:** The chatbot is strictly locked to family and school productivity. If anyone tries to ask it general questions, it will safely refuse to answer by saying, *"I was only developed to answer kid-related questions."*

---

## 3. 🕒 Understanding the Automation Schedule

You do not need to keep any windows open. As long as the 🎯 icon is in the tray, MyTracker is fully automated!

### The Daily Task Sync
At exactly **4:00 PM**, **6:00 PM**, and **8:00 PM** every single day, the app will:
1. Wake up and secretly open your school portal.
2. Read the newest 10-50 unread emails in your inbox.
3. Send all that text to the AI to extract actionable tasks.
4. **Smart Deduplication:** The AI cross-references new tasks against your completed ones. It is smart enough to recognize if a weekly assignment has a new due date, so it creates a new task instead of confusing it for a duplicate!
5. Pop up Brand New Sticky Notes on your desktop for any new homework!

### The Daily Grade Sync
At exactly **5:00 PM** every single day, the app will:
1. Wake up and check your `Grading URL`.
2. Memorize your class averages in the background.
3. If your math grade was a 95 yesterday but is an 88 today, it instantly fires off an alert email to the Parent.

---

## 4. 📝 Using Sticky Notes on the Desktop

When the sync finds homework, it generates digital "Sticky Notes" that float on your desktop.

*   **The Aesthetic:** They look like real paper taped to your monitor with masking tape. They use the Comic Sans font for a handwritten feel.
*   **Color Coding:** High priority tasks are marked with soft pastel red, while standard kid tasks use yellow.
*   **Completing Tasks:** Finished your homework? Just click the **Checkbox** directly on the sticky note. 
    > [!NOTE]
    > The note will vanish instantly, the app will remember that you finished it, and the parent will get an email letting them know you did it!

---

## 5. ✉️ Creating Custom Tasks via Email

You can use natural language to instantly generate new sticky notes! 

1. Open your email app.
2. Send an email to the student's Gmail account with the subject starting with: `MyTracker:`
3. Type out exactly what you want the app to do. 
   - *Example Subject:* `MyTracker: Create a 20 min Music task for every working day until Dec 2026`
4. The AI will read your email, calculate all the exact dates, generate all the necessary tasks, and post them automatically! 
5. **Safety Guardrails:** If the AI detects inappropriate or non-school related instructions in the email, it will safely ignore the command and drop the tasks.

---

## 6. 🎮 Manual Controls & Settings

Sometimes you don't want to wait until 4:00 PM. You can control the app manually at any time by right-clicking the 🎯 icon in the System Tray:

*   **🔄 Sync Now:** Immediately forces the app to read your emails and school portal, bypassing the schedule. New sticky notes will pop up in about 30 seconds.
*   **💬 Chatbot:** Opens the interactive AI support agent.
*   **⚙️ Settings:** Opens the advanced configuration menu if you ever need to manually change your AI model string (e.g. from `gpt-4o-mini` to `gpt-4o`), update your grading URL, or log in to the school portal scraper.
*   **🧹 Clear All Notes:** Temporarily hides all sticky notes from your screen if they are distracting you while playing a game. 
*   **❌ Quit:** Completely shuts down MyTracker and stops all automatic syncing until you relaunch the `.exe`.
