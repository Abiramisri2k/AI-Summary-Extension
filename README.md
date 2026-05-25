# 🧠 AI Summary for Articles — Chrome Extension

A Chrome extension that summarizes any article on the web using the **Google Gemini API**. Get brief, detailed, or bullet-point summaries in seconds — without leaving your tab.

---

## ✨ Features

- 📝 **Brief Summary** — 2-3 sentence overview
- 📄 **Detailed Summary** — Full breakdown of all key points
- 🔹 **Bullet Points** — 5-7 concise key takeaways
- 📋 **Copy to Clipboard** — One-click copy of any summary
- ⚙️ **Secure API Key Storage** — Your Gemini key is saved locally in Chrome

---

## 🚀 Installation (Load Unpacked)

Since this extension is not on the Chrome Web Store, you need to load it manually.

### Step 1 — Clone the Repository

```bash
git clone https://github.com/Abiramisri2k/ai-summary-extension.git
```

Or click **Code → Download ZIP** and extract it.

---

### Step 2 — Open Chrome Extensions Page

In your Chrome browser, go to:

```
chrome://extensions
```

---

### Step 3 — Enable Developer Mode

In the top-right corner of the Extensions page, toggle **Developer mode** ON.

---

### Step 4 — Load the Extension

Click the **"Load unpacked"** button that appears on the top left.

Then select the folder where you cloned/extracted the project.

---

### Step 5 — Get a Gemini API Key

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Sign in with your Google account
3. Click **"Create API Key"**
4. Copy the key

---

### Step 6 — Add Your API Key to the Extension

When the extension loads for the first time, it will automatically open the **Settings page**.

Paste your Gemini API key and click **Save Settings**.

> You can also access settings anytime by right-clicking the extension icon → **Options**.

---

### Step 7 — Use It!

1. Open any article or webpage
2. Click the extension icon in your Chrome toolbar
3. Choose a summary type: **Brief**, **Detailed**, or **Bullet Points**
4. Click **"Summarize"**
5. Wait a few seconds — your summary appears!
6. Click **"Copy"** to copy it to your clipboard

---

## 📁 Project Structure

```
ai-summary-extension/
│
├── manifest.json       # Extension configuration
├── background.js       # Service worker (runs on install)
├── content.js          # Injected into pages to extract article text
├── popup.html          # Extension popup UI
├── popup.js            # Popup logic + Gemini API call
├── options.html        # Settings page UI
├── options.js          # Settings page logic
└── icon.png            # Extension icon
```

---

## ⚙️ Tech Stack

| Part | Technology |
|------|------------|
| Extension | Chrome Manifest V3 |
| AI Model | Google Gemini 2.5 Flash |
| Storage | Chrome Sync Storage |
| Scripting | Vanilla JavaScript |

---

## ❓ Troubleshooting

**"This page cannot be summarized"**
> You are on a Chrome internal page (`chrome://`). Navigate to a real website and try again.

**"Could not extract article text"**
> The page may not have standard article tags. Try refreshing the page and clicking Summarize again.

**"API key not found"**
> Go to the extension Options page and enter your Gemini API key.

**Summary not generating**
> Make sure your API key is valid and active at [Google AI Studio](https://aistudio.google.com).

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 🙌 Contributing

Pull requests are welcome! Feel free to open an issue for bugs or feature requests.

---

## 🎉 Special Thanks

A huge shoutout to [**@RoadsideCoder**](https://www.youtube.com/watch?v=mcfCdFS9VBY) on YouTube for the inspiration and guidance that helped build this project. Go check out the channel — great content for developers! 🙏
