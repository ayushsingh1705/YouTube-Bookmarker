# YouTube Video Bookmarker - Chrome Extension

A Chrome extension that allows users to **bookmark timestamps** in YouTube videos for easy navigation and revisiting. This extension helps you keep track of important moments in videos and return to them instantly.

---
##Demo
![img1](https://github.com/user-attachments/assets/226ba422-af56-47e3-8442-02affc63aec4)
![img2](https://github.com/user-attachments/assets/04981f07-927f-4c38-b4d4-d0f750579c25)
![img3](https://github.com/user-attachments/assets/98d6b293-f815-4579-9824-25f23c4ffbd0)
![img4](https://github.com/user-attachments/assets/23b48b5e-b86d-4bf6-b90e-5b87f219ce36)
![img5](https://github.com/user-attachments/assets/320e8703-375a-48dc-a8eb-4ef1428e75db)


---

## 🚀 Features
- **Bookmark Timestamps**: Save specific points in a YouTube video by clicking a bookmark button.
- **Quick Access**: View saved bookmarks directly from the extension popup.
- **One-Click Navigation**: Jump to bookmarked timestamps instantly.
- **Persistent Storage**: Bookmarks are saved using Chrome's `chrome.storage.sync` and can sync across devices logged into the same Google account.
- **Simple Interface**: Minimal, user-friendly interface with intuitive controls.

---

## 📂 Project Structure
```
📦 youtube-bookmarker-extension
├── assets
│   ├── bookmark.png          // Bookmark icon
│   ├── play.png              // Play icon
│   ├── delete.png            // Delete icon
│   └── ext-icon.png          // Extension icon
├── background.js             // Background script
├── contentScript.js          // Content script injected into YouTube
├── manifest.json             // Chrome extension manifest
├── popup.html                // HTML structure for popup
├── popup.js                  // Logic for handling bookmarks in popup
├── popup.css                 // Styling for popup
└── utils.js                  // Utility functions
```

---

## 🛠️ How It Works
1. **When a YouTube video is loaded**, the extension injects a "Bookmark" button into the video player controls.
2. Clicking the button saves the **current timestamp**.
3. The saved bookmarks can be accessed through the extension popup by clicking on the extension icon.
4. Bookmarks can be played (navigate to that timestamp) or deleted directly from the popup.

---

## 📦 Installation (Running Locally)

1. **Clone this repository**:
2. **Open Chrome** and go to `chrome://extensions/`.
3. Enable **Developer Mode** (toggle at the top-right corner).
4. Click **Load unpacked** and select the cloned project folder.
5. The extension will be installed and appear in your Chrome toolbar.

---

## ⚙️ Usage
1. Open any **YouTube video**.
2. A **bookmark button** will appear in the video player controls.
3. Click the button to save the current timestamp.
4. To view or manage bookmarks, click the extension icon from the toolbar.

---

## 🔧 Configuration and Customization
- **Icons**: Customize the extension icons by replacing the images in the `assets` folder.
- **Popup UI**: Modify `popup.html` and `popup.css` to change the look and feel of the popup.
- **Bookmark Actions**: Enhance bookmark features by modifying `popup.js` or `contentScript.js`.

---


## 🛡️ Security
- Bookmarks are stored using `chrome.storage.sync`, which is tied to the user's Google account and is not accessible by third parties.
- No personal data is collected by this extension.

---

Happy Bookmarking! 🎥

