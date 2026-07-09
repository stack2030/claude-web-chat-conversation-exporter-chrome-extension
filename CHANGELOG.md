# Changelog

## v0.1.1 - 2026-07-09

### Changed

- Updated bundled Claude exporter from v0.1.3 to v0.1.6.
- Replaced old virtualized-DOM scrolling/copy-button export path with fast same-origin Claude conversation data export.
- Improved reliability for large conversations, hundreds of messages, and Claude project chats.
- Removed dependency on mounted visible messages, viewport position, zoom level, and DevTools placement.
- Updated extension documentation, privacy wording, and Chrome Web Store draft text.

### Bundled exporter

- Claude Web Chat Conversation Exporter v0.1.6.

### Privacy model

- No Stack2030 backend.
- No analytics.
- No tracking.
- No third-party upload.
- No remote JavaScript.
- Uses Claude.ai same-origin conversation data available to the active Claude.ai session after explicit user action.
## v0.1.0 - 2026-07

### Added

- Initial Chrome extension baseline.
- Bundled exporter script injection after explicit user click.
- Fast local Markdown download flow using Claude.ai same-origin conversation data.
- No Stack2030 backend, analytics, tracking, or third-party upload.



