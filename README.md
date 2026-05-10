<div align="center">

# 📱 Telegram Downloader

**Automated file download from Telegram (photos, videos, audio, documents, etc.) — no software installation required**

</div>

---

## 📖 Table of Contents

- [✨ Features](#-features)
- [📘 Step-by-Step Guide](#-step-by-step-guide)
- [🧩 Managing Split Files](#-managing-split-files)
- [❓ FAQ](#-faq)

---

## ✨ Features

- 📁 **Supports all file types:** Photos, videos, audio, GIFs, PDFs, ZIP, RAR, documents, etc.
- ✂️ **Smart file splitting:** Automatically splits files larger than your specified threshold
- 🔄 **Simple workflow:** One-time setup, then just a few clicks per download
- 💯 **Completely free:** No API keys or extra registration needed

---

## 📘 Step-by-Step Guide

### Step 1: Log in to GitHub

- Go to [GitHub](https://github.com) and log in to your account.

### Step 2: Fork the Project

1. On the project's main page, click the **Fork** button (top-right).
2. Choose a name for your new repository (e.g., `MyTelegramDownloader`).
3. Click **Create fork**.

### Step 3: Configure Workflow Permissions

> ⚠️ **This step is critical.** Without it, downloaded files won't be saved to your repository.

1. Go to your **forked repository**.
2. Click on the **Settings** tab.
3. In the left menu, click **Actions** → **General**.
4. Scroll down to **Workflow permissions**.
5. Select **Read and write permissions**.
6. Click **Save**.

### Step 4: Enable Actions in Your Forked Repository

1. Go to the **Actions** tab in your repository.
2. If you see a message saying workflows aren't running, click:
   **"I understand my workflows, go ahead and enable them"**

### Step 5: Run the Telegram Downloader

1. In your repository, click the **Actions** tab.
2. In the left sidebar, click **Telegram Downloader**.
3. Click the **Run workflow** button.
4. Fill out the form:

| Field | Description | Example |
|-------|-------------|---------|
| **Telegram link** | Link to the Telegram post | `https://t.me/ChannelName/123` |
| **Split threshold MB** | Max size per file part (0 = no split) | `90` |

5. Click the green **Run workflow** button.

### Step 6: Wait for Completion

- Process typically takes **1–10 minutes** depending on file size.
- You can watch the live progress in the Actions page.
- A **green checkmark ✅** appears when complete.
- A **red ❌** indicates an error.

### Step 7: Find Your Downloaded File

1. Click the **Code** tab in your repository.
2. Open the **downloads** folder.
3. Your downloaded file(s) will be there.

> 📁 **Note:** Non-English filenames are automatically renamed to random English names for GitHub compatibility.

---

## 🧩 Managing Split Files

If the file size exceeds your `Split threshold MB` value, it's split into multiple parts.

**Example:**  
With threshold = 90MB and a 250MB file, you'll get:
- `a1b2c3d4.zip`
- `a1b2c3d4.z01`
- `a1b2c3d4.z02`

**How to extract:**

1. Download **all parts** into the same folder.
2. Right-click **only the `.zip` file**.
3. Select **Extract Here** or **Extract to...**

> ⚠️ **Important:** All parts must be together before extraction, otherwise you'll get an error.

---

## ❓ FAQ

**Q: What file types can be downloaded?**  
A: **Almost all types** — photos, videos, audio, GIFs, PDFs, ZIP, RAR, documents, and more.

**Q: Why isn't the file showing up in my repository?**  
A: Did you complete Step 3 (Read/Write permissions)? That step is essential.

**Q: How long does it take to download?**  
A: Depends on file size. Small files take seconds; large files (multiple GB) may take several minutes.

**Q: Why was the filename changed?**  
A: Non-English filenames are automatically renamed to random English names for GitHub compatibility.

**Q: What if my file is split into multiple parts?**  
A: Download all parts into one folder, then extract only the `.zip` file.

---

## 📋 Quick Summary (Cheatsheet)

| Step | Action |
|------|--------|
| 1 | Log into GitHub |
| 2 | Fork the project |
| 3 | Set Actions permissions to Read/Write |
| 4 | Enable Actions |
| 5 | Click Run workflow and paste Telegram link |
| 6 | Wait for the green checkmark |
| 7 | Find file in the `downloads` folder |
| 8 | If split into parts, extract all together |
