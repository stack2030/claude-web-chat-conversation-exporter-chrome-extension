# Claude Web Chat Conversation Exporter Chrome Extension Documentation

Export Claude.ai web chat conversations locally to Markdown using bundled Claude exporter v0.1.6.

## Current version

Extension: **v0.1.1**  
Bundled exporter: **Claude Web Chat Conversation Exporter v0.1.6**

## Installable extension folder

The installable unpacked Chrome extension is in the repository folder:

```text
extension/
```

Use **that folder** for manual installation.

## Install option 1: Clone/download repo, then Load unpacked

1. Download or clone the repository.
2. Open:

```text
chrome://extensions/
```

3. Turn on **Developer mode**.
4. Click **Load unpacked**.
5. Select:

```text
extension/
```

6. Pin the extension if needed.
7. Open a Claude.ai conversation.
8. Click the extension icon.
9. Click **Export Claude chat**.

## Install option 2: Download release ZIP, extract, then Load unpacked

Chrome cannot load a ZIP directly as an unpacked extension.

1. Download:

```text
claude-web-chat-conversation-exporter-chrome-extension-v0.1.1-unpacked.zip
```

2. Extract the ZIP.
3. Open:

```text
chrome://extensions/
```

4. Turn on **Developer mode**.
5. Click **Load unpacked**.
6. Select the extracted folder containing:

```text
manifest.json
popup.html
popup.js
popup.css
exporters/
icons/
```

## Install option 3: Chrome Web Store

Chrome Web Store publishing is planned.

After approval, install normally from the Chrome Web Store listing.

## Privacy model

- no Stack2030 backend
- no analytics
- no tracking
- no third-party upload
- no remote JavaScript
- bundled exporter code only
- runs only after explicit user action

The extension may make same-origin requests to Claude.ai / Anthropic endpoints available to the active Claude.ai session.

It does not send conversation content to Stack2030 or any unrelated third-party service.

## Project links

GitHub repo:  
https://github.com/stack2030/claude-web-chat-conversation-exporter-chrome-extension

Extension release:  
https://github.com/stack2030/claude-web-chat-conversation-exporter-chrome-extension/releases/tag/v0.1.1

Bundled exporter release:  
https://github.com/stack2030/claude-web-chat-conversation-exporter/releases/tag/v0.1.6