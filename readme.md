# Bookmark Tab Downloader

A Chrome extension to quickly save all your open tabs as bookmarks, or export them as an HTML file for backup.

## Features

- Save all open tabs as bookmarks in a named folder.
- Select specific tabs to save.
- Custom folder name support.
- Context menu integration for quick bookmarking.
- Modern, clean popup UI.

## Installation

1. **Clone or Download this repository.**
2. Open `chrome://extensions` in your browser.
3. Enable **Developer mode** (top right).
4. Click **Load unpacked** and select the project folder.

## Usage

- Click the extension icon to open the popup.
- Enter a folder name (optional).
- Select/deselect tabs as needed.
- Click **Save All Tabs** or **Save Selected** to bookmark.

## Project Structure

```
.
├── background.js
├── manifest.json
├── icons/
│   ├── favicon.png
│   ├── icon.svg
│   ├── icon128.png
│   ├── icon16.png
│   └── icon48.png
└── popup/
    ├── popup.css
    ├── popup.html
    └── popup.js
```

- **background.js**: Handles background tasks, context menu, and bookmark creation.
- **popup/**: Contains the popup UI files.
- **icons/**: Extension icons.

## Permissions

This extension requests the following permissions:

- `bookmarks`: To create and manage bookmarks.
- `tabs`: To read open tabs.
- `downloads`: For exporting bookmarks as HTML (future feature).
- `contextMenus`: For right-click menu integration.

## Development

- Edit the popup UI in [`popup/popup.html`](popup/popup.html), [`popup/popup.js`](popup/popup.js), and [`popup/popup.css`](popup/popup.css).
- Background logic is in [`background.js`](background.js).
- Update [`manifest.json`](manifest.json) for configuration.

## License

MIT License

---
