# Claude Web Chat Conversation Exporter Chrome Extension

**Export Claude.ai web chat conversations locally to Markdown using bundled Claude exporter v0.1.6, without a Stack2030 backend, analytics, tracking, or third-party upload.**

Privacy-first means a Claude-only user should not need an extension that also asks for ChatGPT access.

## Current version

Extension: **v0.1.1**  
Bundled exporter: **Claude Web Chat Conversation Exporter v0.1.6**

## Installable extension folder

The installable unpacked Chrome extension is in:

```text
extension/
```

Use **that folder** when loading the extension manually.

Do not select the whole repository folder if you want the clean installable extension folder.

## What this extension does

1. You open a Claude.ai conversation.
2. You click the browser extension icon.
3. You click **Export Claude chat**.
4. The bundled Claude exporter v0.1.6 runs in the active Claude.ai tab.
5. A local Markdown file downloads.

## Privacy model

- bundled exporter code only
- no remote JavaScript
- no Stack2030 backend
- no analytics
- no tracking
- no third-party upload
- local Markdown download
- runs only after explicit user action
- uses Claude.ai same-origin conversation data available to the active Claude.ai session

The extension may make same-origin requests to Claude.ai / Anthropic endpoints available to the active Claude.ai session as part of exporting the currently open conversation.

It does not send conversation content to Stack2030 or any unrelated third-party service.

## Install option 1: Clone/download repo, then Load unpacked

1. Download or clone this repository.
2. Open Chrome or a Chromium browser.
3. Open:

```text
chrome://extensions/
```

4. Turn on **Developer mode**.
5. Click **Load unpacked**.
6. Select this folder inside the repository:

```text
extension/
```

7. Pin the extension from the browser extensions menu if you want it visible in the toolbar.
8. Open a Claude.ai conversation.
9. Click the extension icon.
10. Click **Export Claude chat**.

## Install option 2: Download release ZIP, extract, then Load unpacked

Chrome cannot load a ZIP directly as an unpacked extension.

Use this flow:

1. Download the release ZIP:

```text
claude-web-chat-conversation-exporter-chrome-extension-v0.1.1-unpacked.zip
```

2. Extract the ZIP to a local folder.
3. Open:

```text
chrome://extensions/
```

4. Turn on **Developer mode**.
5. Click **Load unpacked**.
6. Select the extracted folder that contains:

```text
manifest.json
popup.html
popup.js
popup.css
exporters/
icons/
```

7. Pin the extension if needed.
8. Open a Claude.ai conversation.
9. Click **Export Claude chat**.

## Install option 3: Chrome Web Store

Chrome Web Store publishing is planned.

After approval, the normal install flow will be:

1. Open the Chrome Web Store listing.
2. Click **Add to Chrome**.
3. Open a Claude.ai conversation.
4. Click the extension icon.
5. Click **Export Claude chat**.

## Packed .crx note

Chrome has a **Pack extension** option in `chrome://extensions/` developer mode.

That can create a local `.crx` package, but it is not the recommended public install path. Chrome may warn about or restrict non-store `.crx` installs.

For public users before Chrome Web Store approval, prefer:

```text
Download release ZIP -> extract -> Load unpacked
```

## Folder layout

```text
extension/
├─ manifest.json
├─ popup.html
├─ popup.css
├─ popup.js
├─ exporters/
│  └─ claude-web-chat-conversation-exporter-v0.1.6.js
└─ icons/
   ├─ icon16.png
   ├─ icon32.png
   ├─ icon48.png
   └─ icon128.png
```

## Bundled exporter

This extension bundles:

Claude Web Chat Conversation Exporter v0.1.6  
https://github.com/stack2030/claude-web-chat-conversation-exporter/releases/tag/v0.1.6

v0.1.6 replaced the older virtualized-DOM scrolling/copy-button path with fast same-origin Claude conversation data export.

This improves reliability for:

- large Claude conversations
- project chats
- conversations with hundreds of messages
- different screen sizes
- different browser zoom levels
- different DevTools positions

## Project links

Project page:  
https://stack2030.github.io/claude-web-chat-conversation-exporter-chrome-extension/

Documentation:  
https://stack2030.github.io/claude-web-chat-conversation-exporter-chrome-extension/README.md

GitHub repo:  
https://github.com/stack2030/claude-web-chat-conversation-exporter-chrome-extension

Extension release:  
https://github.com/stack2030/claude-web-chat-conversation-exporter-chrome-extension/releases/tag/v0.1.1

Bundled exporter release:  
https://github.com/stack2030/claude-web-chat-conversation-exporter/releases/tag/v0.1.6

## Security

See:

```text
SECURITY.md
```

Do not paste private conversation content into GitHub issues unless you intentionally choose to share it.

## Disclaimer

This is an independent open-source project by Stack2030.

It is not affiliated with, endorsed by, sponsored by, or officially associated with Anthropic, Claude, OpenAI, or ChatGPT.

## License

MIT License.